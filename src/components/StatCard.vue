<script setup>
import { computed } from 'vue'
import { Package, ShoppingCart, Wallet, TriangleAlert } from 'lucide-vue-next'
const props = defineProps({ label:String, value:[String,Number], subtitle:String, type:String })
const icons = { products: Package, sales: ShoppingCart, revenue: Wallet, alert: TriangleAlert }
const activeIcon = computed(() => icons[props.type] || Package)
</script>
<template><div class="stat-card"><div class="stat-top"><span class="stat-label">{{label}}</span><span class="stat-icon" :class="type"><component :is="activeIcon" :size="19"/></span></div><div class="stat-value">{{value}}</div><div class="stat-sub">{{subtitle}}</div></div></template>
