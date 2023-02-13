<template>
    <v-container class="">
    <v-responsive class="d-flex flex-row align-center fill-height">
        <div class="py-14" />
        <v-row class="d-flex justify-center">
            <v-col>
            <v-card
                class="mx-auto"
                width="100vh"
                variant="outlined"
            >
                <v-card-item>
                    <div>
                        <div class="text-overline mb-1">
                            Aether
                        </div>
                        <div class="text-h6 mb-1">
                        Free Napkins
                        </div>
                        <div class="text-caption">Stuff can go here i guess</div>
                    </div>
                </v-card-item>

                <v-card-actions>
                <v-btn variant="outlined">
                    Button
                </v-btn>
                </v-card-actions>
            </v-card>
        </v-col>
         <v-col>
            <v-card
            class="mx-auto"
            width="40vh"
            variant="outlined"
            prepend-icon="mdi-check-decagram"
            >
                <template v-slot:title>
                Experience
                </template>

                <v-card-text>
                <v-list density="compact" disabled>
                    <v-list-subheader>Savage</v-list-subheader>

                    <v-list-item
                        v-for="(item, i) in savage"
                        :key="i"
                        :value="item"
                        active-color="primary"
                    >
                        <template v-slot:prepend>
                        <v-icon :icon="item.icon"></v-icon>
                        </template>

                        <v-list-item-title v-text="item.text"></v-list-item-title>
                    </v-list-item>

                    <v-list-subheader>Ultimate</v-list-subheader>

                    <v-list-item
                        v-for="(item, i) in ultimate"
                        :key="i"
                        :value="item"
                        active-color="primary"
                    >
                        <template v-slot:prepend>
                        <v-icon :icon="item.icon"></v-icon>
                        </template>

                        <v-list-item-title v-text="item.text"></v-list-item-title>
                    </v-list-item>
                    </v-list>
                </v-card-text>
            </v-card>
            </v-col>
        </v-row>
    </v-responsive>
    </v-container>
</template>

<script lang="ts">
export default {
    data: () => ({
      savage: [
        { text: 'Abyssos Carbuncle', icon: 'mdi-check' },
        { text: 'Abyssos Tree Boss', icon: 'mdi-check' },
        { text: 'Abyssos Funny Man', icon: '' },
        { text: 'Abyssos Boss', icon: 'mdi-check' },
      ],
      ultimate: [
        { text: 'Epic of Alexander', icon: 'mdi-check' },
        { text: 'Dragonsong Fight', icon: '' },
        { text: 'Omegalul Protocal', icon: 'mdi-check' },
      ],
    }),
  }
</script>