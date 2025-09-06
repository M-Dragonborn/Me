<script lang="ts">
	import { faAddressCard } from '@fortawesome/free-solid-svg-icons';
	import SectionHeader from '../components/SectionHeader.svelte';
</script>
<section>
<SectionHeader icon={faAddressCard} text="About Me" />
	<p>
		Hello there! My name is M_Dragonborn. I'm a 22-year-old <span class="highlight">computer science</span>
		student from California.<br />
		My primary career is managing an industrial machinery manufacturing company with my family. As a hobby,
		I work on various open-source community projects, and I also do freelance work periodically.
		I am a gamer & an audiophile who is currently learning programming a bit too seriously. I have knowledge
		in a few different programming languages like
		<span class="highlight">Python</span>,
		<span class="highlight">C</span>, <span class="highlight">HTML</span>, and
		<span class="highlight">CSS</span>, with the first being my most used and the last being my least used
		language.<br/> You can see some of the video games I play on my
		<a class="highlight" href="#steam">Steam</a> account. In addition, I also play <a class="highlight" href="#chess">chess</a> and
		<span class="highlight">Dungeons and Dragons</span>. <span class="highlight">Skyrim</span>, <span class="highlight">The Witcher trilogy</span>, and
		<span class="highlight">Dark Souls</span> are a few of my favorite games. I also enjoy reading, and
		<span class="highlight">the Song of Ice and Fire</span>
		collection is one of my favorites.<br/> (You can probably figure out the obsession with dragons by now).<br/> I generally hang around on
		<a class="highlight" href="#discord">Discord</a> but you can probably find me via
		<a class="highlight" href="#mail">mail</a>.
	</p>
</section>
<style>
    a {
        white-space: nowrap;
    }

    p {
        text-align: justify;
    }
	
    .highlight {
        color: #48a0ff;
    }
	.highlight:hover {
		color: #02ffe1;
		text-shadow: 0 0 8px #02ffe1, 0 0 16px #0084ff;
	}
	
</style>