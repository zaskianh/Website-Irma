<template>
    <div class="container">
        <h2>DOKUMENTASI KEGIATAN <br> IRMA SMKN 4 TASIKMALAYA</h2>
        <div class="content">
            <div class="grid-item">
                <figure>
                    <img src="/assets/img/Mabit_Irma.jpg" alt="Mabit Irma">
                    <figcaption><h3>Mabit Irma</h3></figcaption>
                </figure>
            </div>
            <div class="grid-item">
                <figure>
                    <img src="/assets/img/Pkrm_Irma.jpg" alt="Pkrm Irma">
                    <figcaption><h3>Pkrm Irma</h3></figcaption>
                </figure>
            </div>
            <!-- Kajian Rutin in the center -->
            <div class="grid-item full-width">
                <figure>
                    <img src="/assets/img/Kajian_Rutin.jpg" alt="Kajian Rutin ">
                    <figcaption><h3>Kajian Rutin </h3></figcaption>
                </figure>
            </div>
            <div class="grid-item">
                <figure>
                    <img src="/assets/img/Isra_Miraj.jpg" alt="Isra Mi'raj">
                    <figcaption><h3>Isra Mi'raj</h3></figcaption>
                </figure>
            </div>
            <div class="grid-item">
                <figure>
                    <img src="/assets/img/Pergantian_Irma.jpg" alt="Pergantian Irma">
                    <figcaption><h3>Pergantian Irma</h3></figcaption>
                </figure>
            </div>
        </div>
    </div>
</template>

<style scoped>
    body {
        font-family: Arial, sans-serif;
        background-color: #f5f5f5;
        margin: 0;
        padding: 0;
    }
    .container {
        max-width: 1000px;
        margin: 20px auto;
        background-color: white;
        padding: 20px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        text-align: center;
    }
    h2 {
        color: #007b43;
        font-size: 24px;
        margin-bottom: 20px;
    }
    .content {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 20px;
    }
    @media (max-width: 768px) {
        .content {
            grid-template-columns: 1fr;
        }
    }
    .grid-item {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    /* Full width for Kajian Rutin */
    .grid-item.full-width {
        grid-column: span 2; /* Span across both columns */
    }
    .content img {
        width: 446px;         /* Full width of the grid item */
        height: 228px;      /* Set a fixed height for uniformity */
        object-fit: cover;  /* Ensure the aspect ratio is maintained while covering the area */
        border-radius: 15px;
    }
    .content h3 {
        text-align: center;
        margin-top: 10px;
    }
</style>