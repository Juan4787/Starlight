<script lang="ts">
  import Section from '../ui/Section.svelte';
</script>

<Section className="bg-profundo/10">
  <div class="grid md:grid-cols-[1fr_2fr] gap-8 items-center max-w-4xl mx-auto">
    <div class="relative">
      <div class="aspect-square rounded-full overflow-hidden border-2 border-dorado/20 shadow-xl max-w-[200px] mx-auto">
        <img src="/sabrina-profile.png" alt="Sabrina Meola" class="w-full h-full object-cover" />
      </div>
      <div class="absolute -bottom-2 -right-2 w-12 h-12 bg-dorado/10 rounded-full blur-xl"></div>
    </div>

    <div class="text-center md:text-left">
      <h2 class="text-3xl font-serif font-bold mb-4 text-texto-principal">
        About Sabrina
      </h2>
      <p class="text-lg text-texto-suave leading-relaxed">
        Sabrina Meola wrote this story as a way to share an awakening and redefine God as an intimate experience: guidance, love, and presence.
      </p>
    </div>
  </div>
</Section>
