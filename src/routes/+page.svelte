<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Everything works.Across every device."
	subtitle="Designed to connect effortlessly and elevate what you do."
	imageSrc="/generated/image-a-diverse-group-of-people-gathered-in-a-.webp"
	centered={false}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://logo.clearbit.com/nike.com',
		'https://logo.clearbit.com/target.com',
		'https://logo.clearbit.com/verizon.com'
	]}
/>

<Summary
	title="What we do"
	text="Apple designs and integrates premium hardware, software, and services across iPhone, Mac, iPad, Apple Watch, and more—creating a seamless, intuitive experience for work, play, and everything in between. From streaming on Apple TV+, gaming with Apple Arcade, training with Apple Fitness+, or managing your finances through Apple Card, everything works better together in the Apple ecosystem."
/>

<Testimonials
	testimonials={[
		{
			name: "Greta Lindholm",
			position: "Creative Director",
			company: "Nimbus Agency",
			quote:
				"With MacBook Air, I save hours on every project. My team finishes edits in record time, and our creative flow never gets interrupted.",
			image: "/generated/image-a-confident-middle-aged-woman-working-in.webp"
		},
		{
			name: "Kwame Mansa",
			position: "Music Producer",
			company: "Mansa Soundworks",
			quote:
				"Apple Music lets me manage playlists, share tracks, and relax—all without missing a beat. It makes life and work easier, every day.",
			image: "/generated/image-a-young-black-man-relaxing-in-a-cozy-liv.webp"
		},
		{
			name: "Takeshi Fujimoto",
			position: "Financial Controller",
			company: "Suzukiko Trading Co.",
			quote:
				"Using iPhone to track company expenses minimized budget errors and helped us save thousands this quarter. Real-time control makes all the difference.",
			image: "/generated/image-an-asian-senior-man-thoughtfully-reviewi.webp"
		}
	]}
/>

<Features
	title="Made to work together. Designed to work for you."
	subtitle="Experience seamless integration, privacy, and premium support across every device."
	features={[
	  {
	    title: "Smart assistance, right when you need it",
	    description: "Apple Intelligence helps you write, organize, and get things done—automatically. All while keeping your data private and your information secure."
	  },
	  {
	    title: "All your devices, all in sync",
	    description: "Start an email on your iPhone, finish it on your Mac, then join a FaceTime call from your iPad—no setup needed, it just works."
	  },
	  {
	    title: "Your entertainment, your way",
	    description: "Stream award-winning shows on Apple TV+, listen to over 100 million songs on Apple Music, and play hundreds of ad-free games with Apple Arcade—all in one ecosystem."
	  },
	  {
	    title: "Power that keeps up with you",
	    description: "From the performance of M-series chips to the all-day battery life of Apple Watch, every product is engineered to run fast, cool, and smooth no matter the task."
	  },
	  {
	    title: "Finance designed around you",
	    description: "With Apple Card’s daily cash back, flexible payment options, and seamless Wallet integration, you’re in control of spending, saving, and sharing—and staying on budget feels effortless."
	  },
	  {
	    title: "Support that never misses a beat",
	    description: "Whether you need directions, a repair, or advice on what to buy next, Apple Support makes it easy to get expert help—online, by chat, or in-store whenever you need it."
	  }
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Pick up right where you left off",
			description: "Start an email on your Mac, reply from your iPad, and finish it from your iPhone without missing a beat. With Apple's seamless handoff across devices, it's easy to stay in sync wherever you go.",
			image: "/generated/image-a-group-of-people-gathered-in-a-cozy-liv.webp",
			link: {
				href: "/use-cases/device-integration",
				label: "Learn more"
			}
		},
		{
			title: "Entertainment made for everyone",
			description: "Share Apple TV+, Apple Arcade, and Apple Music with your family while keeping individual preferences and privacy intact. Family sharing makes it simple to manage it all from one place.",
			image: "/generated/image-a-family-of-four-sitting-together-in-a-s.webp",
			link: {
				href: "/use-cases/family-entertainment",
				label: "Learn more"
			}
		},
		{
			title: "Daily wellness that stays with you",
			description: "Track workouts with Apple Watch, view progress over time on your iPhone, and stay motivated with Fitness+ wherever you are. Your health goals, always connected and easy to follow.",
			image: "/generated/image-an-active-person-jogging-along-a-scenic-.webp",
			link: {
				href: "/use-cases/daily-wellness",
				label: "Learn more"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction
  title="Designed to work smarter, together"
  subtitle="Every device. Every service. All Apple."
  description="Experience beautiful design, seamless integration, and rewarding experiences across iPhone, Mac, iPad, Apple Watch, and more. Join millions who work, play, and create with Apple—where everything just works."
  imageSrc="/generated/image-a-cheerful-college-student-sitting-comfo.webp"
  callsToAction={[
    { href: '/shop', label: 'Shop now', variant: 'primary' },
    { href: '/learn', label: 'Learn more', variant: 'secondary' }
  ]}
/>
