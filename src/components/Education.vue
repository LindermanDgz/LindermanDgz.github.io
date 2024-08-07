<template>
    <v-container>
        <v-row>
            <v-col cols="12" class="text-center">
                Education
            </v-col>
            <v-col cols="12" lg="1" xl="2" xxl="3"> </v-col>
            <v-col>
                <v-card variant="flat">
                    <v-row class="text-center" align="stretch" justify="center">
                        <v-col cols="3">
                            <v-img v-if="$vuetify.theme.name === 'light'" src="@/assets/unach_light.png"></v-img>
                            <v-img v-else src="@/assets/unach.svg"></v-img>
                        </v-col>
                        <v-col>
                            <v-card-title>Universidad Autónoma de Chiapas</v-card-title>
                            <v-card-subtitle>2009 - 2014</v-card-subtitle>
                            <v-card-text>
                                <v-icon icon="mdi-rocket-launch"></v-icon> B.S. Physics</v-card-text>
                        </v-col>
                    </v-row>
                </v-card>
            </v-col>
            <v-col>
                <v-card variant="flat">
                    <v-row class="text-center" align="stretch" justify="center">
                        <v-col cols="3">
                            <v-img src="@/assets/upchiapas.png" color="white" rounded="circle"></v-img>
                        </v-col>
                        <v-col>
                            <v-card-title>Universidad Politécnica de Chiapas</v-card-title>
                            <v-card-subtitle>2017 - 2020</v-card-subtitle>
                            <v-card-text>
                                <v-icon icon="mdi-desktop-classic"></v-icon> B.E. Software Engineering</v-card-text>
                        </v-col>
                    </v-row>
                </v-card>
            </v-col>
            <v-col cols="12" lg="1" xl="2" xxl="3"> </v-col>
        </v-row>
    </v-container>
</template>
