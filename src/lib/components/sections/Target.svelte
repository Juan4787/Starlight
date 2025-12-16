<script lang="ts">
  import Section from '../ui/Section.svelte';
  import Card from '../ui/Card.svelte';
</script>

<Section className="bg-profundo/20">
  <div class="text-center mb-16">
    <h2 class="text-3xl md:text-4xl font-serif font-bold mb-6 text-texto-principal">
      If you ever felt you needed to come back to yourself... <span class="block text-dorado mt-2">it is for you.</span>
    </h2>
  </div>

  <div class="grid md:grid-cols-2 gap-6 max-w-4xl mx-auto">
    <Card className="hover:-translate-y-1 transition-transform duration-300">
      <div class="flex items-start gap-4">
        <div class="w-12 h-12 rounded-full bg-dorado/10 flex items-center justify-center shrink-0 text-2xl">
          🌙
        </div>
        <div>
          <h3 class="text-xl font-serif font-bold text-texto-principal mb-2">Mom / Dad</h3>
          <p class="text-texto-suave">A reading ritual for sleeping in calm.</p>
        </div>
      </div>
    </Card>

    <Card className="hover:-translate-y-1 transition-transform duration-300">
      <div class="flex items-start gap-4">
        <div class="w-12 h-12 rounded-full bg-dorado/10 flex items-center justify-center shrink-0 text-2xl">
          ✨
        </div>
        <div>
          <h3 class="text-xl font-serif font-bold text-texto-principal mb-2">Sensitive adults</h3>
          <p class="text-texto-suave">A story that feels like meditation.</p>
        </div>
      </div>
    </Card>

    <Card className="hover:-translate-y-1 transition-transform duration-300">
      <div class="flex items-start gap-4">
        <div class="w-12 h-12 rounded-full bg-dorado/10 flex items-center justify-center shrink-0 text-2xl">
          🌱
        </div>
        <div>
          <h3 class="text-xl font-serif font-bold text-texto-principal mb-2">Teachers / guides</h3>
          <p class="text-texto-suave">A loving conversation starter.</p>
        </div>
      </div>
    </Card>

    <Card className="hover:-translate-y-1 transition-transform duration-300">
      <div class="flex items-start gap-4">
        <div class="w-12 h-12 rounded-full bg-dorado/10 flex items-center justify-center shrink-0 text-2xl">
          🕊️
        </div>
        <div>
          <h3 class="text-xl font-serif font-bold text-texto-principal mb-2">Seekers</h3>
          <p class="text-texto-suave">Simple spirituality, without rigidity.</p>
        </div>
      </div>
    </Card>
  </div>
</Section>
