<script>
import Button from '../reusable/Button.vue';
export default { components: { Button } };
</script>

<template>
	<div class="w-full md:w-1/2">
		<div
			class="leading-loose max-w-xl m-4 p-7 bg-secondary-light dark:bg-secondary-dark rounded-xl shadow-sm text-left"
		>
			<p
				class="font-general-medium text-primary-dark dark:text-primary-light text-3xl mb-8"
			>
				Formulaire
			</p>
			<form action="#" class="font-general-regular space-y-7">
				<div>
					<label
						class="block text-lg text-primary-dark dark:text-primary-light mb-2"
						for="name"
						>Nom & Prénom(s)</label
					>
					<input
						class="w-full px-5 py-2 border border-gray-300 dark:border-primary-dark border-opacity-50 text-primary-dark dark:text-secondary-light bg-ternary-light dark:bg-ternary-dark rounded-md shadow-sm text-md"
						id="name"
						name="name"
						type="text"
						required=""
						placeholder="Votre Nom & Prénom(s)"
						aria-label="Name"
					/>
				</div>
				<div>
					<label
						class="block text-lg text-primary-dark dark:text-primary-light mb-2"
						for="email"
						>Email</label
					>
					<input
						class="w-full px-5 py-2 border border-gray-300 dark:border-primary-dark border-opacity-50 text-primary-dark dark:text-secondary-light bg-ternary-light dark:bg-ternary-dark rounded-md shadow-sm text-md"
						id="email"
						name="email"
						type="text"
						required=""
						placeholder="Votre adresse mail"
						aria-label="Email"
					/>
				</div>
				<div>
					<label
						class="block text-lg text-primary-dark dark:text-primary-light mb-2"
						for="subject"
						>Sujet</label
					>
					<input
						class="w-full px-5 py-2 border border-gray-300 dark:border-primary-dark border-opacity-50 text-primary-dark dark:text-secondary-light bg-ternary-light dark:bg-ternary-dark rounded-md shadow-sm text-md"
						id="subject"
						name="subject"
						type="text"
						required=""
						placeholder="Sujet du message"
						aria-label="Subject"
					/>
				</div>

				<div>
					<label
						class="block text-lg text-primary-dark dark:text-primary-light mb-2"
						for="message"
						>Message</label
					>
					<textarea
						class="w-full px-5 py-2 border border-gray-300 dark:border-primary-dark border-opacity-50 text-primary-dark dark:text-secondary-light bg-ternary-light dark:bg-ternary-dark rounded-md shadow-sm text-md"
						id="message"
						name="message"
						cols="14"
						rows="6"
						placeholder="Votre message ici"
						aria-label="Message"
					></textarea>
				</div>

				<div>
					<Button
						title="Envoyer Message"
						class="px-4 py-2 text-white font-bold tracking-wider bg-indigo-500 hover:bg-indigo-600 focus:ring-1 focus:ring-indigo-900 rounded-lg duration-500 rounded-full"
						type="submit"
						aria-label="Envoyer Message"
					/>
				</div>
			</form>
		</div>
	</div>
</template>

<style lang="scss" scoped></style>
