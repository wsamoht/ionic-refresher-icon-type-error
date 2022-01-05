<template>
    <ion-page>
        <ion-header :translucent="true">
            <ion-toolbar>
                <ion-title>IonRefresherContent Icon TypeError</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content :fullscreen="true">
            <IonRefresher slot="fixed">
                <IonRefresherContent />
            </IonRefresher>
            <div style="text-align: center; padding: 20px">
                <p>
                    Emulate iOS and refresh the tab to see the error in the
                    console.
                </p>
                <p>
                    "Uncaught TypeError: Failed to construct 'URL': Invalid base
                    URL"
                </p>
            </div>
        </ion-content>
    </ion-page>
</template>

<script lang="ts">
import {
    IonContent,
    IonHeader,
    IonPage,
    IonRefresher,
    IonRefresherContent,
    IonTitle,
    IonToolbar,
} from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
    components: {
        IonContent,
        IonHeader,
        IonPage,
        IonRefresher,
        IonRefresherContent,
        IonTitle,
        IonToolbar,
    },
});
</script>