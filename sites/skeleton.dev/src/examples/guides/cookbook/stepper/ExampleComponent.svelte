<script lang="ts">
	import ExampleStepOne from './ExampleStepOne.svelte';

	// Source Data
	const steps = [
		{ component: ExampleStepOne, props: { label: 'Step 1' } }
		// ...
	];
</script>

<!-- <Stepper> -->
{#each steps as step}
	<!-- 1. Dynamically render the step component. -->
	<!-- 2. Spread the component props. -->
	<step.component {...step.props} />
{/each}
<!-- </Stepper> -->
