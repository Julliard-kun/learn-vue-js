<template>
    <header>
        <nav>
            <NuxtLink to="/products">Products Merch</NuxtLink>
        </nav>
    </header>

    <!-- Content will be inserted here -->
    <div>
        <slot />
    </div>

    <footer>
        <ul>
            <li>
                <NuxtLink to="/dashboard">Dashboard</NuxtLink>
            </li>
            <li>
                <NuxtLink to="/products">Products</NuxtLink>
            </li>
            <li>
                <NuxtLink to="/">Logout</NuxtLink>
            </li>
        </ul>
    </footer>
</template>