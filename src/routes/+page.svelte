<script lang="ts">
    import AmptLogo from "$lib/images/ampt.svg";
</script>

<svelte:head>
    <title>Ampt + Svelte</title>
    <meta name="description" content="Ampt + Svelte Demo App" />
</svelte:head>

<body>
    <div class="container">
        <div class="column">
            <div class="circle">
                <img
                    style="align-self: center;"
                    src={AmptLogo}
                    alt="Ampt Logo"
                    width="150"
                    height="150"
                />
            </div>
            <h5>Welcome to Svelte on Ampt!</h5>
        </div>
    </div>
</body>

<style>
    @import url("https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap");
    @import url("https://fonts.googleapis.com/css?family=Source+Code+Pro:400,700&display=swap");

    h5 {
        font-family: "Montserrat", sans-serif;
        font-weight: 400;
        font-size: 1.5rem;
        color: #fff;
        text-align: center;
        margin: 0;
        padding: 0;
    }

    body {
        margin: 0;
        padding: 0;
        font-family: sans-serif;
        background: #000;
    }

    .column {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-content: center;
    }

    .circle {
        border-radius: 50%;
        background-color: #fff;
        padding: 30px;
        margin: 20px;
        align-self: center;
        display: flex;
        align-content: center;
        justify-content: center;
        width: 20;
        height: 20;
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
    }

    .container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-content: center;
        background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
        background-size: 400% 400%;
        animation: gradient 15s ease infinite;
        height: 100vh;
        width: 100vw;
        overflow: hidden;
    }

    @keyframes gradient {
        0% {
            background-position: 0% 50%;
        }
        50% {
            background-position: 100% 50%;
        }
        100% {
            background-position: 0% 50%;
        }
    }
</style>
