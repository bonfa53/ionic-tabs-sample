<template>
	<ion-page>
		<ion-header>
			<ion-toolbar>
				<ion-buttons slot="start">
					<ion-back-button/>
				</ion-buttons>
				<ion-title size="large">Tab 2</ion-title>
			</ion-toolbar>
		</ion-header>
		<ion-content :fullscreen="true">
			<div style="display:flex; flex-direction:column; align-items:center; justify-content:center; height:100%">
				<h1>TAB 2</h1>
				<ion-button @click="navigate">Navigate to child</ion-button>
			</div>
		</ion-content>
	</ion-page>
</template>
<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, useIonRouter, IonButton, IonButtons, IonBackButton } from '@ionic/vue';

const router = useIonRouter();
function navigate() {
	router.push('/tabs/tab2/child');
}
</script>
