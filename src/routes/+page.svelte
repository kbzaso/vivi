<script>
	const info = {
		title: 'Viaje con confianza, explore con facilidad',
		description: 'Agente de viajes',
		image: '/hero-big.jpg',
		url: 'https://vivipalominos.com',
		cta: 'Planifica tu viaje ahora',
		ctaWsp: 'https://wa.me/5699974471',
		agent: {
			name: 'Viviana Palominos',
			photo: '/agent.png',
			email: 'vivi@vivipalominos.com',
			phone: '+569 9997 4471'
		}
	};
</script>

<svelte:head>
	<title>Vivi Palominos - Agente de viajes</title>
</svelte:head>

<main class="bg-cloud relative mx-auto flex h-dvh items-center justify-center">
	<nav class="absolute top-0 z-10 w-full bg-white/20 p-4 backdrop-blur-sm">
		<div class="container mx-auto flex items-center justify-between">
			<img src="/isologo.svg" alt="Logo de vivipalominos.com" class="w-12 h-12" />
			<a
				href={info.ctaWsp}
				target="_blank"
				class="bg-night mt-4 w-fit rounded-full px-4 py-2 text-white md:mt-0">Hablemos por Whatsapp</a
			>
		</div>
	</nav>
	<header class="absolute top-0 z-0 w-full">
		<picture>
			<source srcset="/hero-big.webp" type="image/webp" />
			<img src="/hero-big.jpg" alt="Hero" class="h-[500px] w-full object-cover" />
		</picture>
		<!-- AIRPLAIN -->
		<div>
			<img
				src="/airplain.png"
				class="absolute top-20 right-0 z-20 w-80 md:top-10 md:right-36 md:w-[600px]"
				alt=""
				aria-hidden="true"
			/>
		</div>
		<!-- AGENT + TEXT -->
		<div class="absolute md:top-[400px] top-[350px] px-4 z-10 w-full">
			<div class="flex flex-col space-y-4 space-x-8 md:flex-row max-w-7xl mx-auto">
				<picture class="">
					<img src="/agent.png" class="h-56 w-48 object-cover md:h-96 md:w-56" alt="" />
				</picture>
				<div class="flex flex-col">
					<h1 class="mt-4 text-4xl font-extrabold md:w-[800px] md:text-7xl">
						{info.title}
					</h1>
					<div class="mt-4 flex flex-col md:flex-row md:space-x-4">
						<span class="text-2xl">{info.agent.name}</span>
						<span class="hidden text-lg md:block">{info.agent.email}</span>
						<span class="hidden text-lg md:block">{info.agent.phone}</span>
					</div>
					<button class="bg-water mt-4 w-fit rounded-lg px-4 py-2 ">{info.cta}</button>
				</div>
			</div>
		</div>
		<!-- SEPARATOR DESKTOP -->
		<div class="absolute right-0 -bottom-36 hidden w-full rotate-6 md:block">
			<img src="/separator.svg" class="w-full object-contain" alt="" aria-hidden="true" />
		</div>
		<!-- SEPARATOR MOBILE -->
		<div class="absolute -bottom-72 w-full md:hidden">
			<!-- This image is decorative and serves as a visual separator -->
			<img src="/separator-sm.svg" class="w-full" alt="" role="separator" aria-hidden="true" />
		</div>
	</header>
</main>

<style>
</style>
