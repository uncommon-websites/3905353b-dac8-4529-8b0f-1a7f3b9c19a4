<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
  testimonials={[
    {
      name: "Declan Myers",
      position: "Product designer",
      company: "Studio North",
      quote:
        "Switching from PC to my MacBook Air boosted my productivity overnight—I spend less time troubleshooting and more time creating.",
      image:
        "/generated/image-professional-headshot-of-a-young-white-m.webp"
    },
    {
      name: "Rebekah Tran",
      position: "CFO",
      company: "Crestway Tech",
      quote:
        "The Apple Card mobile experience is beyond seamless. It’s the first credit card I’ve actually enjoyed using.",
      image:
        "/generated/image-professional-headshot-of-a-vietnamese-wo.webp"
    },
    {
      name: "Malcolm Quinn",
      position: "Director of operations",
      company: "Forge AV",
      quote:
        "Apple TV+ is hands down the most consistent content library—we replaced three other services with it and never looked back.",
      image:
        "/generated/image-professional-headshot-of-a-black-man-ope.webp"
    }
  ]}
/>

<CallToAction
  title="People love how it all just works"
  subtitle="From setup to everyday use, Apple products stay in sync—so you can enjoy more, worry less, and smile sooner."
  description="Get started today and feel the difference."
  imageSrc="/generated/image-a-joyful-person-sitting-comfortably-in-a.webp"
  callsToAction={[
    { href: '/shop', label: 'Shop now', variant: 'primary' },
    { href: '/learn', label: 'See our offers', variant: 'secondary' }
  ]}
/>

