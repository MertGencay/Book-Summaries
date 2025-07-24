<template>
    <section>
        <div class="container">
            <SectionHeader title="Kitap Ayrıntıları" text="Deneme"></SectionHeader>
            <button>Geri</button>
            <div class="row mb-4">
                <div class="col-lg-6">
                    <img class="card-img-top" src="../../images/b_detail.jpg">
                </div>
                <div class="col-lg-6 details-wrapper">
                    <p class="lead description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Et, ex accusamus cum sequi officia quasi?</p>
                    <div class="mb-4">
                        <div class="row border-bottom pb-2">
                            <div class="col-lg-6"><strong>Sayfa</strong></div>
                            <div class="col-lg-6">278</div>
                        </div>
                        <div class="row border-bottom pb-2">
                            <div class="col-lg-6"><strong>Kategori</strong></div>
                            <div class="col-lg-6">Roman</div>
                        </div>
                        <div class="row border-bottom pb-2">
                            <div class="col-lg-6"><strong>Puanı</strong></div>
                            <div class="col-lg-6">7.2</div>
                        </div>
                        <div class="row border-bottom pb-2">
                            <div class="col-lg-6"><strong>Yükleme Tarihi</strong></div>
                            <div class="col-lg-6">24 Temmuz 2025</div>
                        </div>
                    </div>
                    <div class="comments-section">
                        <h3 class="display-6 mb-2">Yorumlar</h3>
                        <div class="card mb-4">
                            <div class="card-body">
                                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis, eaque!</p>
                                <div class="d-flex justify-content-between">
                                    <p class="fw-bold fst-italic">Deneme</p>
                                    <div class="d-flex align-items-center">
                                        <p>Beğenme</p>
                                        <p class="ps-2"><strong>8</strong></p>
                                    </div>
                                </div>
                            </div> 
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import SectionHeader from '@/components/SectionHeader.vue';

    export default {
        name: "BookDetailView",
        components:{
            SectionHeader
        }
    }
</script>

<style scoped>
.details-wrapper{
    max-height: 740px;
    display: flex;
    flex-direction: column;
}

.comments-section{
    flex-grow: 1;
    overflow-y: auto;
}

.description{
    min-height: 150px;
    max-height: 250px;
    overflow-y: auto;
}
</style>