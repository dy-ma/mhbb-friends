<script lang="ts">
	import { Button } from '$lib/components/ui/button/index';
	import * as Accordion from '$lib/components/ui/accordion/index';
	import { Separator } from '$lib/components/ui/separator/index';
	import temple from '$lib/images/temple.jpg';
	import * as Card from '$lib/components/ui/card/index.js';
	import { AspectRatio } from '$lib/components/ui/aspect-ratio';
</script>

<main class="mx-auto flex flex-col font-serif">
	<div class="mt-20 flex h-dvh flex-col items-center justify-between">
		<div>
			<h1 class="text-center text-6xl"><a href="/">Keiro Kai</a></h1>
			<h2 class="text-center text-xl">Morgan Hill Buddhist Community Center</h2>
		</div>

		<div class="flex w-full flex-col">
			<div class="relative h-[50vh] w-full overflow-hidden">
				<img src={temple} alt="temple" class="absolute inset-0 h-full w-full object-cover" />
			</div>
			<span class="ml-auto mr-6 text-right"
				>Photo of church dedication, October 15, 1967 provided by Jeremy Aragaki.</span
			>
		</div>

		<Button variant="secondary" href="#details" class="font-semibold">Learn More</Button>
		<div id="details"></div>
	</div>

	<div class="max-w-3xl self-center p-4">
		<div class="py-10">
			<h1 class="mb-2 text-4xl">
				Keiro Kai means <span class="rounded-sm bg-primary p-1 text-primary-foreground block sm:inline w-fit"
					>Respect for the Aged</span
				>
			</h1>
			<p class="min-w-60">
				Keiro Kai is our way of honoring the seniors within our community. This special occasion is
				filled with joy, gratitude, and heartwarming moments as we recognize and appreciate the
				wisdom, experience, and contributions of our elders.
			</p>
		</div>

		<div class="my-8">
			<div class="flex h-full items-center text-sm">
				<span class="text-4xl">
					Join us
					<span class="underline"> January 25th, 2025 at 12PM </span>
				</span>
			</div>
			<p>We invite you to join us for a day of festivities, including:</p>
			<ul class="list-disc pl-5">
				<li>
					<span class="font-bold">Delicious Food:</span> Savor a delectable lunch prepared with care.
				</li>
				<li>
					<span class="font-bold">Games and Activities:</span> Participate in engaging games and activities
					designed for all ages.
				</li>
				<li>
					<span class="font-bold">Special Recognition:</span> Honor our esteemed seniors with special
					awards and acknowledgements.
				</li>
			</ul>
		</div>
		<h1 id="directions" class="text-4xl">How to Attend</h1>

		<Accordion.Root type="single" class="mb-6">
			<Accordion.Item value="item-1">
				<Accordion.Trigger>When is the event?</Accordion.Trigger>
				<Accordion.Content>Saturday, January 25th, 2025 at 12PM</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-2">
				<Accordion.Trigger>Where is the event?</Accordion.Trigger>
				<Accordion.Content
					>The Morgan Hill Buddhist Community Center Annex. The Address is 16450 Murphy Ave. Look
					for signage for "Keiro Kai Parking".</Accordion.Content
				>
			</Accordion.Item>
			<Accordion.Item value="item-3">
				<Accordion.Trigger>Which building is the Annex?</Accordion.Trigger>
				<Accordion.Content
					>The Annex is located behind the main Temple. Signage will be posted to direct you.</Accordion.Content
				>
			</Accordion.Item>
			<Accordion.Item value="item-4">
				<Accordion.Trigger>Do I need to buy tickets?</Accordion.Trigger>
				<Accordion.Content>I don't know.</Accordion.Content>
			</Accordion.Item>
		</Accordion.Root>

		<div class="flex flex-col md:flex-row">
			<div class="relative w-full overflow-hidden pt-[56%]">
				<iframe
					class="absolute bottom-0 left-0 right-0 top-0 h-full w-full rounded-xl"
					style="border:0"
					title="16450 Murply Ave"
					loading="lazy"
					allowfullscreen
					src="https://www.google.com/maps/embed/v1/place?q=place_id:ChIJJQzJm4HfkYARIhW23t_U6y0&key=AIzaSyDgQ7wfwWUyk_DNiCBx4DXn2K_DAjTM7Uc"
				></iframe>
			</div>
		</div>
	</div>
</main>
