<template>
    <v-container>
        <v-row class="text-center">
            <v-col>
                Job Experience
            </v-col>
        </v-row>
        <v-row>
            <v-timeline side="end" align="start" truncate-line="start">
                <v-timeline-item v-for="(role, i) in roles" :key="i" dot-color="blue-lighten-3" fill-dot
                    icon="mdi-briefcase" :icon-color="$vuetify.theme.name === 'light' ? 'white' : 'black'" width="100%">
                    <template v-slot:opposite>
                        <v-card-text v-text="role.date">
                        </v-card-text>
                    </template>
                    <v-card variant="tonal">
                        <v-card-title v-text="role.name">
                        </v-card-title>
                        <v-card-subtitle>
                            <v-icon icon="mdi-domain"></v-icon> <v-text v-text="role.company"></v-text>
                            <v-spacer></v-spacer>
                            <v-icon icon="mdi-map-marker"></v-icon> <v-text v-text="role.work_model"></v-text>
                        </v-card-subtitle>
                        <v-card-text v-text="role.description"></v-card-text>
                    </v-card>
                </v-timeline-item>
            </v-timeline>
        </v-row>
    </v-container>
</template>

<script>
export default {
    data() {
        return {
            roles: [
                {
                    name: 'Software Engineer',
                    company: 'Oracle Corporation',
                    date: 'Sep 2024 - Present',
                    description: "Oracle Linux YUM Service",
                    work_model: "Remote",
                },
                {
                    name: 'Software Engineer',
                    company: 'Intel Corporation',
                    date: 'Jan 2022 - Jul 2023',
                    description: "RTL Development and CI/CD",
                    work_model: "Remote",
                },
                {
                    name: 'Graduate Technical Intern',
                    company: 'Intel Corporation',
                    date: 'Nov 2020 - Nov 2021',
                    description: "RTL Development and CI/CD",
                    work_model: "Remote",
                },
                {
                    name: 'Back End Python Developer',
                    company: 'Universidad Intercultural de Chiapas',
                    date: 'Sep 2020 - Dec 2020',
                    description: "RESTful API development with Django framework RESTful API development with Django framework RESTful API development with Django framework",
                    work_model: "Remote",
                },
                {
                    name: 'Fullstack Developer Angular',
                    company: 'Adiante Apps',
                    date: 'May 2020 - Sep 2020',
                    description: "WEB and Mobile application development using Angular",
                    work_model: "Remote",
                },
            ],
        }
    },
}
</script>