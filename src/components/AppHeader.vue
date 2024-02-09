<script>
export default {
    data() {
        return {
            genders: [
                {
                    gender: 'Donna',
                },
                {
                    gender: 'Uomo',
                },
                {
                    gender: 'Bambini',
                }

            ],
            icons: [
                {
                    iconName: 'fa-regular fa-user'
                },
                {
                    iconName: 'fa-regular fa-heart'
                },
                {
                    iconName: 'fa-solid fa-cart-shopping'
                }
            ]
        };
    }
};
</script>
<template>
    <header class="header">
        <div class="container">
            <div class="header-nav-left">
                <ul>
                    <li v-for="sex in genders"><a href="#">{{ sex.gender }}</a></li>

                </ul>
            </div>
            <div class="header-logo-center">
                <img class="logo" src="../assets/img/boolean-logo.png" alt="" />
            </div>
            <div class="header-nav-right">
                <ul>
                    <li v-for="icone in icons">
                        <a href="#" :class="icone.iconName"></a>
                    </li>

                </ul>
            </div>
        </div>
    </header>
</template>
<style lang="scss">
.header {
    width: 100%;
    background-color: #ff6900;
    height: 80px;
    display: flex;
    align-items: center;

    .container {
        display: flex;
        justify-content: space-between;
        width: 1200px;
        margin-left: 300px;

        a {
            text-decoration: none;
            color: white;
            padding: 10px;
        }

        .header-nav-left ul {

            list-style-type: none;
            text-align: center;
            margin: 0 10px;
            vertical-align: middle;
            line-height: 130px;
        }

        .header-nav-left li {
            display: inline-block;
            text-align: center;
            vertical-align: middle;
            padding: 20px;
            color: white;
        }

        .logo {
            vertical-align: middle;
            width: 200px;
            padding: 70px;
            display: flex;
            justify-content: center;

        }

        .header-nav-right ul {
            list-style-type: none;
            line-height: 100px;
        }

        .header-nav-right li {
            display: inline-block;
            vertical-align: middle;
            padding: 20px;
        }


    }
}
</style>