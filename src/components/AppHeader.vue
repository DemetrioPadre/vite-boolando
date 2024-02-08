<script>
export default {};
</script>
<template>
    <header class="header">
        <div class="container">
            <div class="header-nav-left">
                <ul>
                    <li><a href="#">Donna</a></li>
                    <li><a href="#">Uomo</a></li>
                    <li><a href="#">Bambini</a></li>
                </ul>
            </div>
            <div class="header-logo-center">
                <img class="logo" src="./img/boolean-logo.png" alt="" />
            </div>
            <div class="header-nav-right">
                <ul>
                    <li>
                        <a href="#"><i class="fa-regular fa-user"></i></a>
                    </li>
                    <li>
                        <a href="#"><i class="fa-regular fa-heart"></i></a>
                    </li>
                    <li>
                        <a href="#"><i class="fa-solid fa-bag-shopping"></i></a>
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
    min-height: 80px;
    position: fixed;
    display: flex;
    justify-content: right;
    z-index: 2;
    align-items: center;

    .container {
        display: flex;
        justify-content: space-between;
        width: 1200px;
        margin-left: 300px;

        .header-nav-left ul {

            list-style-type: none;
            text-align: center;
            margin: 0 10px;
            vertical-align: middle;
        }

        .header-nav-left li {
            display: inline-block;
            text-align: center;
            vertical-align: middle;
            padding: 20px;
        }

        .logo {
            vertical-align: middle;
            width: 200px;
            padding: 20px;
            display: flex;
            justify-content: center;
        }

        .header-nav-right ul {
            list-style-type: none;
        }

        .header-nav-right li {
            display: inline-block;
            vertical-align: middle;
            padding: 20px;
        }


    }
}
</style>