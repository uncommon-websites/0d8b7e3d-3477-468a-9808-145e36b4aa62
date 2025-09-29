<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Precision",
			description: "Every dataset we create meets the exacting standards required for production AI systems."
		},
		{
			title: "Understanding",
			description: "We immerse ourselves in your operational workflows to create datasets that actually work."
		},
		{
			title: "Transformation",
			description: "We don't just process data—we unlock the AI automation potential hiding in your business."
		}
	];
</script>

<SecondaryHero
	title="From raw data to AI automation powerhouse"
	subtitle="We transform medium-sized businesses by converting their big data into precisely labeled training datasets"
	imageSrc="/generated/image-a-diverse-group-of-professionals-collabo.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We exist because 70% of data engineers spend their time on tedious manual labeling instead of building breakthrough AI models. This isn't just inefficient—it's preventing the next wave of AI innovation.",
		"Medium-sized businesses sit on goldmines of operational data, but lack the infrastructure to transform it into the precisely labeled datasets that fuel AI automation. We bridge this gap.",
		"Our approach is different: we understand the operational workflows that generic AI platforms miss. We don't just label data—we create training datasets that actually work in real manufacturing environments.",
		"Every dataset we create brings companies closer to true AI automation. We measure success not in labels processed, but in the autonomous systems our clients deploy and the human potential they unlock."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- Team and investors sections removed as no team members or investors information is available -->

<!-- CTA Section -->
<CallToAction
	title="Ready to scale your AI?"
	subtitle="Transform your data into training gold"
	description="Join the medium-sized businesses already turning their big data chaos into precisely labeled datasets that power breakthrough AI automation."
	imageSrc="/generated/image-a-professional-data-engineer-smiling-at-.webp"
/>
