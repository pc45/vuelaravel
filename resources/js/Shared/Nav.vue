<template>
    <nav class="">
        <ul class="flex list-none space-x-6 list-inside">
            <li><Link
                href="/"
                class="text-blue-500 hover:underline"
                :class="{'font-bold underline': $page.component === 'Home'}">
                Home</Link></li>
            <li><Link href="/users?foo=bar" class="text-blue-500 hover:underline"  :class="{'font-bold underline': $page.component === 'Users'}">Users</Link></li>
            <li><Link href="/settings" class="text-blue-500 hover:underline"  :class="{'font-bold underline': $page.component === 'Settings'}">Settings</Link></li>
            <li><Link href="/logout" method="post" as="button" class="text-blue-500 hover:underline">Logout</Link></li>
        </ul>
    </nav>
</template>

<script>

export default {
  name: 'Nav'
};
</script>

<style scoped>

</style>
