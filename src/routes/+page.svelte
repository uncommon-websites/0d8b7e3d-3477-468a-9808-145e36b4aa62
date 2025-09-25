<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	centered={false}
	title="Turn messy data into real outcomes"
	subtitle="Build models faster with labeled datasets that work"
	imageSrc="/generated/image-a-data-engineer-sits-confidently-at-a-sp.webp"
/>
<LogoScroller 
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/shopify.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/dropbox.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/zillow.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/reddit.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Nakamura",
			position: "Senior Data Engineer",
			company: "MedDevice Manufacturing",
			quote:
				"We went from spending 6 weeks manually labeling quality control images to having clean datasets ready in 3 days. Our AI model accuracy improved from 73% to 94%, and we saved $180K in the first quarter alone by catching defects earlier in production.",
			image: "/generated/image-a-professional-asian-woman-with-a-confid.webp"
		},
		{
			name: "Carlos Rodriguez",
			position: "Head of Data Operations",
			company: "Precision Logistics",
			quote:
				"Before this platform, our team was drowning in unlabeled shipping data. Now we process 10x more datasets with 40% fewer resources. The automated labeling reduced our model deployment time from 4 months to 6 weeks, helping us capture a $2.3M contract we would have lost otherwise.",
			image: "/generated/image-a-professional-hispanic-man-with-a-confi.webp"
		},
		{
			name: "Keisha Williams",
			position: "AI Implementation Lead",
			company: "AutoParts Direct",
			quote:
				"The risk of deploying untested AI models kept me up at night. Their labeled datasets gave us confidence to automate our inventory predictions. We reduced stockouts by 65% and overstock by 45%, translating to $890K in working capital savings within 8 months.",
			image: "/generated/image-a-professional-black-woman-with-a-confid.webp"
		}
	]}
/>

<Features
	title="Transform raw data into AI-ready datasets"
	subtitle="Reduce labeling time by 85% with workflow-aware automation designed for manufacturing and quality control teams"
	features={[
		{
			title: "Workflow-aware auto-labeling",
			description: "Our AI understands your manufacturing processes and automatically labels quality control data with 94% accuracy. Focus on building models, not labeling data."
		},
		{
			title: "Manufacturing-specific models",
			description: "Pre-trained on 50M+ industrial datasets covering defect detection, assembly validation, and quality metrics. Start with models that already understand your domain."
		},
		{
			title: "Seamless pipeline integration",
			description: "Connect directly to your existing data systems with APIs that understand operational workflows. No complex migrations or workflow disruptions required."
		},
		{
			title: "Enterprise performance at mid-market cost",
			description: "Get the same labeling quality as Scale AI at 60% lower cost with pricing designed for 500-2000 employee companies. Scale your AI initiatives without breaking budgets."
		},
		{
			title: "Real-time quality validation",
			description: "Every labeled dataset is validated against your specific quality standards with instant feedback loops. Catch labeling errors before they impact model training."
		},
		{
			title: "Collaborative annotation platform",
			description: "Enable your entire data engineering team to review, approve, and refine labels together with role-based permissions and audit trails."
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
