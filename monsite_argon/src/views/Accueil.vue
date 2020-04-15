<template>
    <!-- <section class="section section-lg section-shaped overflow-hidden my-0"> -->
    <section style="background-color: #212529;">    
                    <b-carousel id="carousel1"
                                v-model="slide"
                                :interval="4000"
                                controls
                                indicators
                                background="#212529"
                                img-width="1024"
                                img-height="480"
                                style="text-shadow: 1px 1px 2px #333; padding: 20px;">

                        <!-- Text slides with image -->
                        <b-carousel-slide
                        caption="First slide"
                        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                        img-src="img/accueil/dybala.jpg">
                        </b-carousel-slide>

                        <b-carousel-slide
                        caption="Second slide"
                        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                        img-src="img/accueil/varane.jpg">
                        </b-carousel-slide>

                        <b-carousel-slide
                        caption="Third slide"
                        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                        img-src="img/accueil/ligue1.jpg">
                        </b-carousel-slide>
                    </b-carousel>
            <p></p>
            <b-container class="bv-example-row">                
                <b-row>
                    <b-col cols="12" md="4" class="text-center">
                        <img v-lazy="'img/accueil/klopp.jpg'" alt="Raised circle image"
                            class=" rounded-circle shadow-lg" style="width: 150px;">
                        <h2>Klopp se méfie de l'Atlético</h2>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna.</p>
                        <p><a class="btn btn-secondary" href="#" role="button">View details &raquo;</a></p>                           
                    </b-col>
                    <b-col cols="12" md="4" class="text-center">
                        <img v-lazy="'img/accueil/real.jpg'" alt="Raised circle image"
                            class="img-fluid rounded-circle shadow-lg" style="width: 150px;">
                        <h2>Zidane évoque le cas Gareth Bale.</h2>
                        <p>Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Cras mattis consectetur purus sit amet fermentum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh.</p>
                        <p><a class="btn btn-secondary" href="#" role="button">View details &raquo;</a></p>        
                    </b-col>
                    <b-col cols="12" md="4" class="text-center">
                        <img v-lazy="'img/accueil/chelsea.jpg'" alt="Raised circle image"
                            class="img-fluid rounded-circle shadow-lg" style="width: 150px;">
                        <h2>Chelsea tombe face au Red Devils</h2>
                        <p>Donec sed odio dui. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Vestibulum id ligula porta felis euismod semper. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.</p>
                        <p><a class="btn btn-secondary" href="#" role="button">View details &raquo;</a></p>                       
                    </b-col>              
                </b-row>

                <hr class="featurette-divider">
                <div class="row featurette">
                <div class="col-md-7">
                    <h2 class="featurette-heading"><span class="text-muted">Tuchel brouille les pistes avant Dortmund</span></h2>
                    <p class="lead">Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl consectetur. Fusce dapibus, tellus ac cursus commodo.</p>
                </div>
                <div class="col-md-5">
                    <img src="img/accueil/tuchel.jpg" width="100%" height="100%" alt="">
                </div>
                </div>
                <hr class="featurette-divider">        
                <div class="row featurette">
                <div class="col-md-7 order-md-2">
                    <h2 class="featurette-heading"><span class="text-muted">"Je dirais que mon équipe favorite est le Barça"</span></h2>
                    <p class="lead">Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl consectetur. Fusce dapibus, tellus ac cursus commodo.</p>
                </div>
                <div class="col-md-5 order-md-1">
                    <img src="img/accueil/trentaa.jpg" width="100%" height="100%" alt="">
                </div>
                </div>        
                <hr class="featurette-divider">            
                <div class="row featurette">
                <div class="col-md-7">
                    <h2 class="featurette-heading"><span class="text-muted"> Terim, entraîneur de Galatasaray, testé positif au COV-19</span></h2>
                    <p class="lead">Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl consectetur. Fusce dapibus, tellus ac cursus commodo.</p>
                </div>
                <div class="col-md-5">
                    <img src="img/accueil/fatih.jpg" width="100%" height="100%" alt="">
                </div>
                </div>

                <div class="article">
                    <div class="embed">
                    <b-embed
                    style="padding: 35px;"
                    type="iframe"
                    aspect="16by9"
                    src="https://www.youtube.com/embed/JGUOzrdW8jE"
                    allowfullscreen
                    ></b-embed>
                    </div>

                    <div class="list-group">
                    <b-list-group style="padding-bottom: 20px">
                    <b-list-group-item href="#" active class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                        <h5 class="mb-1">List group item heading</h5>
                        <small>3 days ago</small>
                        </div>

                        <p class="mb-1">
                        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
                        </p>

                        <small>Donec id elit non mi porta.</small>
                    </b-list-group-item>

                    <b-list-group-item href="#" class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                        <h5 class="mb-1">List group item heading</h5>
                        <small class="text-muted">3 days ago</small>
                        </div>

                        <p class="mb-1">
                        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
                        </p>

                        <small class="text-muted">Donec id elit non mi porta.</small>
                    </b-list-group-item>
                    <b-list-group-item href="#" class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                        <h5 class="mb-1">List group item heading</h5>
                        <small class="text-muted">3 days ago</small>
                        </div>

                        <p class="mb-1">
                        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
                        </p>

                        <small class="text-muted">Donec id elit non mi porta.</small>
                    </b-list-group-item>
                    <b-list-group-item href="#" class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                        <h5 class="mb-1">List group item heading</h5>
                        <small class="text-muted">3 days ago</small>
                        </div>

                        <p class="mb-1">
                        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
                        </p>

                        <small class="text-muted">Donec id elit non mi porta.</small>
                    </b-list-group-item>
                    <b-list-group-item href="#" class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                        <h5 class="mb-1">List group item heading</h5>
                        <small class="text-muted">3 days ago</small>
                        </div>

                        <p class="mb-1">
                        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
                        </p>

                        <small class="text-muted">Donec id elit non mi porta.</small>
                    </b-list-group-item>
                    <b-list-group-item href="#" class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                        <h5 class="mb-1">List group item heading</h5>
                        <small class="text-muted">3 days ago</small>
                        </div>

                        <p class="mb-1">
                        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
                        </p>

                        <small class="text-muted">Donec id elit non mi porta.</small>
                    </b-list-group-item>

                    <b-list-group-item href="#" disabled class="flex-column align-items-start">
                        <div class="d-flex w-100 justify-content-between">
                        <h5 class="mb-1">Disabled List group item</h5>
                        <small class="text-muted">3 days ago</small>
                        </div>

                        <p class="mb-1">
                        Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
                        </p>

                        <small class="text-muted">Donec id elit non mi porta.</small>
                    </b-list-group-item>
                    </b-list-group>
                    
                    </div>

                </div>
            </b-container>         
    </section>  
</template>

<script>
import { BCarousel } from "bootstrap-vue/esm/components/carousel/carousel";
import { BCarouselSlide } from "bootstrap-vue/esm/components/carousel/carousel-slide";
import { CarouselPlugin } from 'bootstrap-vue'
import { BCard } from "bootstrap-vue/esm/components/card";
import { BContainer, BCol, BRow } from "bootstrap-vue/esm/components/layout";
import { BEmbed } from "bootstrap-vue";
import { BListGroup } from "bootstrap-vue";
import { BListGroupItem } from "bootstrap-vue";

export default {
  components: {
    BCarousel,
    BCarouselSlide,
    CarouselPlugin,
    BCard,
    BContainer,
    BCol,
    BRow,
    BEmbed,
    BListGroup,
    BListGroupItem
  }
};
</script>
