<script lang="ts">
    import { QRCodeImage } from "svelte-qrcode-image";
    let links_url = "https://links.angs.dev/";
</script>

<div class="container">
    <div class="qr-container">
        <QRCodeImage text={links_url} width={600} height={600} />
    </div>
</div>

<style>
    :global(body) {
        background: #2e3541;
        font-family: Arial, sans-serif;
        margin: 0;
    }

    .container {
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
    }

    .qr-container {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>
