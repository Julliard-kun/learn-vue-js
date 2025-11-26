<template>
    <header>
        <nav>
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
        </nav>
    </header>

    <!-- Content will be inserted here -->
    <div>
        <slot />
    </div>
</template>