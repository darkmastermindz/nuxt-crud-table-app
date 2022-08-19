<template>
    <div class="col-12">
        <div class="card card-w-title">
            <Menubar :model="items">
                <template #start>
                    <span>
                        <p-menuitem-icon>
                           <Logo/>
                        </p-menuitem-icon>
                    </span>
                </template>
                <template #end>
                    <span class="p-input-icon-left">
                        <i class="pi pi-search" />
                        <InputText type="text" placeholder="Search" />
                    </span>
                </template>
            </Menubar>
        </div>
    </div>

</template>

<script>
import Menubar from 'primevue/menubar';
import Logo from './Logo.vue';

export default {
    data() {
        return {
            items: [
                {
                    label: "Nuxt Crud Table App"
                },
                {
                    label: "Logout",
                    icon: "pi pi-fw pi-power-off"
                },
            ]
        };
    },
    components: { Logo }
}
		
</script>

<style lang="scss" scoped>

</style>