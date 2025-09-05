<script lang="ts">
	import { faAddressCard } from '@fortawesome/free-solid-svg-icons';
	import SectionHeader from '../components/SectionHeader.svelte';
</script>
<section>
<SectionHeader icon={faAddressCard} text="About Me" />
	<p>
		Hi im M_Dragonborn Or Musfiq Drake whichever way you know me im a 22-year-old <span class="highlight">CS</span> student From California.<br>
		I run a industrial machine manufactering company with my family as my primary career and work on various small communitry projects as a hobby
		and occasionally do freelance work.
    	I am a audiophile & a gamer whos Currently learning programming a bit too seriously.
    	I have knowledge in a few differnet programming languages like
    	<span class="highlight">Python</span>,
    	<span class="highlight">C</span>, <span class="highlight">HTML</span> and <span class="highlight">CSS</span>,
    	with the
    	first being my most and last being my least used languages.I try to enjoy my free time by playing videogames some of which you can see on my <a class="highlight" href="#steam">steam</a> I also play <a class="highlight" href="#chess">chess</a> and <span class="highlight">Dungeons and Dragons</span>.
		some of my favourite games include ,<span class="highlight">Skyrim</span>, <span class="highlight">The Witcher series</span>, and <span class="highlight">Dark Souls</span>. I also love reading books my favourite being <span class="highlight">Song of Ice and Fire</span> series. (hence the obsession with dragons)
		I generally hang around on
		<a class="highlight" href="#discord">discord</a> but you can probably find me via <a class="highlight" href="#mail">mail</a>.
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
	
</style>