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
                        <v-col>
                            <v-avatar class="ma-3" rounded="0" size="100">
                                <v-img v-if="$vuetify.theme.name === 'light'" src="@/assets/unach_light.png"></v-img>
                                <v-img v-else src="@/assets/unach.svg"></v-img>
                            </v-avatar>
                        </v-col>
                        <v-col>
                            <v-card-title>Universidad Autónoma de Chiapas</v-card-title>
                            <v-card-subtitle>Aug 2009 - Dec 2014</v-card-subtitle>
                            <v-card-text>Physics</v-card-text>
                        </v-col>
                    </v-row>
                </v-card>
            </v-col>
            <v-col>
                <v-card variant="flat">
                    <v-row class="text-center" align="stretch" justify="center">
                        <v-col>
                            <v-avatar class="ma-3" rounded="50" size="100" color="white">
                                <v-img src="@/assets/upchiapas.png"></v-img>
                            </v-avatar>
                        </v-col>
                        <v-col>
                            <v-card-title>Universidad Politécnica de Chiapas</v-card-title>
                            <v-card-subtitle>Jan 2017 - Dec 2020</v-card-subtitle>
                            <v-card-text>Physics</v-card-text>
                        </v-col>
                    </v-row>
                </v-card>
            </v-col>
            <v-col cols="12" lg="1" xl="2" xxl="3"> </v-col>
        </v-row>
    </v-container>
</template>
