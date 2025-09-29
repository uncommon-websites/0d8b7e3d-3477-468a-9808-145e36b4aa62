<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		[key: string]: any;
	} = $props();
</script>

<header class="relative overflow-hidden border-b border-gray-100 dark:border-gray-900" {...rest}>
	<!-- Gradient Background -->
	<div class="absolute inset-0 bg-gradient-to-br from-gray-900 via-gray-900 to-primary-900 opacity-95"></div>
	<div class="absolute inset-0 bg-gradient-to-t from-secondary-950/20 to-transparent"></div>
	
	<div class="relative section-px section-py container mx-auto">
		<div class="grid gap-12 lg:grid-cols-2 lg:gap-16 items-center">
			<!-- Content Section -->
			<div class="space-y-8">
				<div class="space-y-4">
					<h1 class="text-display font-[450] tracking-tight text-white">
						{title}
					</h1>
					<p class="text-title3 text-gray-300 leading-relaxed">
						{subtitle}
					</p>
				</div>
				
				<!-- Mission Statement -->
				<div class="space-y-2">
					<p class="text-callout text-gray-400 leading-relaxed">
						Every day, data engineers spend 70% of their time manually labeling data instead of building AI models. 
						We change that by turning your raw data into precisely labeled training datasets, unlocking the AI potential your business deserves.
					</p>
				</div>
			</div>
			
			<!-- Image Section -->
			<div class="relative">
				<div class="aspect-[4/3] overflow-hidden rounded-xl bg-gray-800 shadow-2xl">
					<img
						class="h-full w-full object-cover transition-transform duration-700 hover:scale-105"
						src={imageSrc}
						alt="Team collaboration representing our mission-driven culture"
					/>
				</div>
				
				<!-- Decorative Elements -->
				<div class="absolute -top-4 -right-4 h-24 w-24 bg-gradient-to-br from-primary-500 to-secondary-500 rounded-full opacity-20 blur-xl"></div>
				<div class="absolute -bottom-4 -left-4 h-32 w-32 bg-gradient-to-br from-secondary-600 to-primary-600 rounded-full opacity-15 blur-2xl"></div>
			</div>
		</div>
	</div>
</header>
