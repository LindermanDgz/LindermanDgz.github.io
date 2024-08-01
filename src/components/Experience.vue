<template>
    <v-timeline side="end">
        <v-timeline-item v-for="(role, i) in roles" :key="i" dot-color="blue-lighten-3" icon="mdi-star" size="large"
            fill-dot>
            <template v-slot:opposite>
                <div class="pt-1 headline font-weight-light" v-text="role.date"></div>
            </template>
            <div>
                <h2 class="mt-n1 headline font-weight-light mb-4" v-text="role.name"></h2>
                <div v-text="role.company"> </div>
            </div>
        </v-timeline-item>
    </v-timeline>
</template>

<script>
export default {
    data: () => ({
        roles: [
            {
                name: 'Software Engineer',
                company: 'Intel Corporation',
                date: 'Jan 2022 - Jul 2023',
            },
            {
                name: 'Graduate Technical Intern',
                company: 'Intel Corporation',
                date: 'Nov 2020 - Nov 2021',
            },
            {
                name: 'Back End Python Developer',
                company: 'Universidad Intercultural de Chiapas',
                date: 'Sep 2020 - Dec 2020',
            },
            {
                name: 'Fullstack Developer Angular',
                company: 'Adiante Apps',
                date: 'May 2020 - Sep 2020',
            },
        ],
    }),
}
</script>