<script lang="ts">
	import { Button } from '$lib/components/ui/button/index';
	import * as Carousel from '$lib/components/ui/carousel/index';
	import { AspectRatio } from '$lib/components/ui/aspect-ratio/index';
	import * as Accordion from '$lib/components/ui/accordion/index';
</script>

<main class="mx-auto flex max-w-3xl flex-col p-6 font-serif">
	<div class="mt-20 flex h-dvh flex-col items-center justify-between">
		<div>
			<h1 class="text-center text-6xl"><a href="/">Keiro Kai</a></h1>
			<h2 class="text-center text-xl">Morgan Hill Buddhist Community Center</h2>
		</div>
		<Carousel.Root class="w-full max-w-lg">
			<Carousel.Content>
				{#each [1, 2, 3] as num}
					<Carousel.Item
						><AspectRatio
							ratio={16 / 9}
							class="flex w-full items-center justify-center rounded-md bg-muted"
							><span class="text-4xl">{num}</span></AspectRatio
						></Carousel.Item
					>
				{/each}
			</Carousel.Content>
			<Carousel.Previous />
			<Carousel.Next />
		</Carousel.Root>

		<Button variant="secondary" href="#details" class="font-semibold">Learn More</Button>
		<div id="details"></div>
	</div>

	<div class="py-10">
		<div class="">
			<h1 class="text-4xl">Saturday, January 25th, 2025 at 12PM</h1>
		</div>
		<p class="min-w-60">
			Keiro Kai, meaning "Respect for the Aged" in Japanese, is a traditional Japanese celebration
			honoring seniors within our community. This special occasion is filled with joy, gratitude,
			and heartwarming moments as we recognize and appreciate the wisdom, experience, and
			contributions of our elders.
		</p>
	</div>

	<div class="my-8">
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
				<span class="font-bold">Special Recognition:</span> Honor our esteemed seniors with special awards
				and acknowledgements.
			</li>
		</ul>
	</div>
	<h1 id="directions" class="text-4xl">How to Attend</h1>
	<div class="flex flex-col md:flex-row">
		<div class="relative w-full overflow-hidden pt-[56%]">
			<iframe
				class="rounded-md absolute top-0 bottom-0 right-0 left-0 w-full h-full"
				style="border:0"
				title="16450 Murply Ave"
				loading="lazy"
				allowfullscreen
				src="https://www.google.com/maps/embed/v1/place?q=place_id:ChIJJQzJm4HfkYARIhW23t_U6y0&key=AIzaSyDD-7DFU337aeI1PRCspQqxdx1bR4Y9dQE"
			></iframe>
		</div>
		<Accordion.Root type="single" class="ml-6 w-full sm:max-w-[30%]">
			<Accordion.Item value="item-1">
				<Accordion.Trigger>When is the event?</Accordion.Trigger>
				<Accordion.Content>Saturday, January 25th, 2025 at 12PM</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-2">
				<Accordion.Trigger>How do I get to the Temple?</Accordion.Trigger>
				<Accordion.Content>
					The Address is 16450 Murphy Ave.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-3">
				<Accordion.Trigger>Do I need to buy tickets?</Accordion.Trigger>
				<Accordion.Content>
					I don't know.
				</Accordion.Content>
			</Accordion.Item>
		</Accordion.Root>
	</div>

	<p class="my-10">
		Lorem ipsum odor amet, consectetuer adipiscing elit. Varius orci egestas leo bibendum natoque
		nunc. Enim sed donec varius netus duis turpis cras tellus maecenas. Ultrices tristique ultricies
		pellentesque litora orci sollicitudin. Arcu lacinia ut cursus velit venenatis mus quam suscipit
		mus. Consequat duis in nisl interdum dictumst aliquam semper. Habitant nullam efficitur eu cras
		dolor porta lobortis? Quis aliquet ultrices sodales ligula himenaeos in urna. Ligula tincidunt
		sociosqu fringilla fusce; suspendisse euismod duis. Sapien ante ultrices habitasse ante auctor.
		In cubilia vehicula ac mi ridiculus rhoncus. Facilisi suscipit primis hendrerit mauris congue
		mattis. Tempor viverra dapibus nam volutpat est; eros fermentum elit. Aliquet sed primis
		fermentum ipsum pretium commodo. Feugiat at justo id potenti euismod himenaeos volutpat
		imperdiet aptent. Sapien risus aptent praesent vivamus id. Leo diam suspendisse cursus
		adipiscing neque torquent aliquet. Finibus fringilla elit montes, hendrerit bibendum neque
		class. Curabitur tortor conubia non porttitor parturient nisl feugiat auctor. Phasellus
		condimentum commodo amet in aliquet parturient. Velit fermentum netus quisque erat quam pharetra
		venenatis. Felis neque lectus facilisis himenaeos mus ullamcorper rutrum penatibus. Nam
		imperdiet justo bibendum in adipiscing cras auctor. Enim dictum malesuada donec pulvinar est
		turpis vitae feugiat bibendum. Massa lacinia interdum est magnis curabitur sollicitudin gravida
		massa integer. Gravida primis viverra commodo facilisis pellentesque eu nisi. Ornare tempor
		sapien dapibus ultrices mattis feugiat dolor odio phasellus? Rhoncus malesuada potenti ac magna
		tristique. Viverra in dictumst parturient enim penatibus nullam. Eget vivamus finibus dolor
		consequat ligula nec nam. Porttitor pharetra pretium per interdum massa ante aenean urna eget.
		Eleifend turpis volutpat vulputate faucibus tortor pretium et. Donec ultrices efficitur duis
		tortor eros; euismod ultricies ullamcorper. Nisl est scelerisque suspendisse nulla libero tellus
		faucibus urna. Purus ridiculus tincidunt nam vulputate a. Velit quisque fusce arcu orci feugiat
		aliquet neque lacus. Potenti feugiat himenaeos est eleifend sollicitudin elementum pellentesque
		nam cursus. Ullamcorper quam rutrum ultricies aliquet dictumst in gravida lacus finibus.
	</p>
</main>
