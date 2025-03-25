<svelte:head>
	<title>Vivi Palominos - Agente de viajes</title>
</svelte:head>

<main class="bg-cloud relative mx-auto flex h-dvh items-center justify-center">
	<nav class="absolute top-0 z-10 w-full bg-white/20 p-4 backdrop-blur-sm">
		<div class="container mx-auto flex items-center justify-between">
			<img src="/logo.svg" alt="Logo de vivipalominos.com" class="w-60" />
			<button>Whatsapp</button>
		</div>
	</nav>
	<header class="absolute top-0 z-0 w-full">
		<picture>
			<source srcset="/hero-big.webp" type="image/webp" />
			<img src="/hero-big.jpg" alt="Hero" class="h-[500px] w-full object-cover" />
		</picture>
        <!-- AIRPLAIN -->
        <div>
            <img src="/airplain.png" class="absolute z-20 top-20 w-80 right-0 md:right-36 md:top-10 md:w-[600px]" alt="" aria-hidden="true">
        </div>
        <!-- SEPARATOR DESKTOP -->
		<div class="absolute -bottom-36 hidden md:block w-full rotate-6 right-0">
			<img src="/separator.svg" class="w-full object-contain" alt="" aria-hidden="true" />
		</div>
        <!-- SEPARATOR MOBILE -->
        <div class="absolute -bottom-72 md:hidden w-full">
            <!-- This image is decorative and serves as a visual separator -->
            <img src="/separator-sm.svg" class="w-full" alt="" role="separator" aria-hidden="true" />
		</div>
	</header>
</main>
