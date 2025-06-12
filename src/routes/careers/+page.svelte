<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
  {
    title: "Impact at scale",
    description:
      "Shape devices, software, and services that touch millions every day—worldwide.",
    icon: IconBriefcase,
  },
  {
    title: "Exceptional growth",
    description:
      "Learn and innovate alongside industry leaders, with room to move and advance.",
    icon: IconUsers,
  },
  {
    title: "Apple-style benefits",
    description:
      "Enjoy product discounts, wellness support, and comprehensive coverage, all from day one.",
    icon: IconHeart,
  },
];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior Frontend Developer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Backend Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Design Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "UX/UI Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Analyst",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Marketing
		{
			title: "Marketing Specialist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Strategist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Social Media Manager",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
  {
    name: "Alexei Bennett",
    position: "Product Manager",
    company: "Software Engineering",
    quote:
      "There’s an openness here I haven’t found anywhere else. People care not just about your job but about how you're growing—personally and professionally. Within three years, I moved from analyst to product lead.",
    image: "/generated/image-a-professional-headshot-of-alexei-a-whit.webp"
  },
  {
    name: "Nadira Kapur",
    position: "UI Designer",
    company: "Apple Watch Team",
    quote:
      "Whether I'm brainstorming a new watch face or troubleshooting early builds, I’m constantly collaborating with people who bring out my best ideas. The creative support and real trust mean everything in a fast-paced environment.",
    image: "/generated/image-a-professional-headshot-of-nadira-a-sout.webp"
  },
  {
    name: "Emilio Ramirez",
    position: "Retail Specialist",
    company: "Apple Store Walnut Creek",
    quote:
      "What surprised me most? How well life and work coexist here. I'm able to take care of customers in the morning and still make it to my kid’s soccer game thanks to flexible scheduling.",
    image: "/generated/image-a-professional-headshot-of-emilio-a-lati.webp"
  }
];

	const processSteps = [
  {
    step: 1,
    title: "Apply online",
    description: "Upload your resume and supporting work—help us get to know the real you.",
  },
  {
    step: 2,
    title: "Virtual interview",
    description: "We schedule a short call to understand your strengths and interests.",
  },
  {
    step: 3,
    title: "Team interview(s)",
    description: "Meet future teammates to discuss collaboration, creativity, and skills.",
  },
  {
    step: 4,
    title: "Offer and onboarding",
    description: "If it’s a match, we’ll help you get started and support you at every step.",
  },
];

	const values = [
  {
    icon: IconHeart,
    title: "Ideas matter more than titles",
    description:
      "Original thinking is at the heart of every breakthrough. We give people room to voice bold ideas, wherever they come from.",
  },
  {
    icon: IconUsers,
    title: "Build with rigor, deliver with heart",
    description:
      "We craft products with deep attention to quality, always focused on real human impact.",
  },
  {
    icon: IconGlobe,
    title: "Think bigger—together",
    description:
      "Collaboration across disciplines lets us push boundaries and create remarkable things as a team.",
  },
];
</script>

<!-- Hero Section -->

<SecondaryHero
  title="Create what’s next together"
  subtitle="Work with impact, grow through creativity and collaboration"
  imageSrc="/generated/image-a-modern-office-environment-featuring-a-.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Build your career while making an impact" />

	<div class="mt-16 grid gap-4 md:grid-cols-3">
		{#each benefits as benefit}
			<Card {...benefit} />
		{/each}
	</div>
</section>

<!-- Culture Section -->
<Culture {values} />

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Our application process</h2>

		<div class="grid gap-12 md:grid-cols-3">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
