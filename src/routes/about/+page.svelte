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
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
		}
	];
</script>

<SecondaryHero
	title="Designed to work as one"
	subtitle="Every product works beautifully together—with you at the center."
	imageSrc="/mockups/airport-screen-1749720379500.png"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Apple began in a garage in 1976, when Steve Jobs, Steve Wozniak, and Ronald Wayne set out to build computers people could actually use. Their goal was simple but bold: make technology more personal, more intuitive, and beautifully designed. That philosophy hasn’t changed—it’s why Apple products started with simple beginnings and sparked a global shift in how people think about and interact with technology.",
		"From the first Mac to the iPhone, iPad, Apple Watch, and Apple TV, innovation has fueled every decision. But it’s not just about features—it’s about creating experiences that feel effortless. Apple has always focused on the person in front of the screen, building devices and software that work better together. Whether you’re listening to music, collaborating on a project, or closing your activity rings, the seamless connection across devices is designed to feel like second nature.",
		"Today, Apple is part of everyday life for millions around the world. Our commitment to quality, privacy, and sustainability drives everything we do, from custom silicon to recycled materials in our devices. And we continue to grow not as a company that just makes products—but as a connected ecosystem built to support creativity, learning, fitness, entertainment, and financial wellbeing. It all connects back to a simple idea: technology should work for you."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<section class="founders">
  <h1 class="mb-4">The team that started it all</h1>
  <h2 class="mb-2">Behind every product, a bold beginning</h2>
  <p class="mb-8">Apple was founded by three individuals driven by curiosity, creativity, and the belief that technology should be accessible, personal, and empowering.</p>
  <div class="founders-section grid grid-cols-1 md:grid-cols-3 gap-8 mb-16">
    <div class="founder-card text-center">
      <img src="/generated/image-a-charismatic-individual-in-a-studio-por.webp" alt="Steve Jobs headshot" class="object-cover rounded-lg mb-4 w-full h-auto" />
      <h3 class="text-lg font-semibold">Steve Jobs</h3>
      <p class="text-sm text-secondary mb-2">Co-founder & visionary leader</p>
      <p class="text-base">Steve pushed Apple forward with his unique ability to merge technology and design. His focus on simplicity and user experience continues to shape everything we make.</p>
    </div>
    <div class="founder-card text-center">
      <img src="/generated/image-a-cheerful-person-smiling-in-a-professio.webp" alt="Steve Wozniak headshot" class="object-cover rounded-lg mb-4 w-full h-auto" />
      <h3 class="text-lg font-semibold">Steve Wozniak</h3>
      <p class="text-sm text-secondary mb-2">Co-founder & engineering pioneer</p>
      <p class="text-base">Woz designed and built Apple’s first computers, setting the technical foundation for the company. His dedication to innovation and efficiency still resonates across our products.</p>
    </div>
    <div class="founder-card text-center">
      <img src="/generated/image-a-professional-individual-in-a-suit-capt.webp" alt="Ronald Wayne headshot" class="object-cover rounded-lg mb-4 w-full h-auto" />
      <h3 class="text-lg font-semibold">Ronald Wayne</h3>
      <p class="text-sm text-secondary mb-2">Co-founder</p>
      <p class="text-base">Ron played a key early role in establishing Apple's legal and operational structure. He helped draft the company’s first partnership agreement in 1976.</p>
    </div>
  </div>
  <h2 class="mb-2">Shaped by people. Redefined by ideas.</h2>
  <p>From a small garage in California to homes and hands across the world, Apple was built on a belief: that great ideas, powered by collaboration and design, can change everything.</p>
</section>





<!-- CTA Section -->
<CallToAction
	title="Help shape what’s next"
	subtitle="Build products millions love"
	description="At Apple, you don’t just create products—you help build the future. Whether you're a designer, engineer, or student just getting started, your ideas can make a lasting impact on the way people connect, learn, and live. Our teams thrive on collaboration, curiosity, and pushing past what’s expected."
	callsToAction={[
		{
			href: "/careers",
			label: "See open roles",
			variant: "primary"
		},
		{
			href: "/internships",
			label: "Explore student programs",
			variant: "secondary"
		}
	]}
/>
