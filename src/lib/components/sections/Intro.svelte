<script lang="ts">
  import Section from '../ui/Section.svelte';
  import Card from '../ui/Card.svelte';
</script>

<Section className="bg-gradient-to-b from-noche to-profundo/30">
  <div class="text-center max-w-3xl mx-auto mb-16">
    <h2 class="text-3xl md:text-4xl font-serif font-bold mb-6 text-texto-principal">
      A story about remembering.
    </h2>
    <p class="text-lg text-texto-suave leading-relaxed">
      Long ago, deep in the universe, there was a great Light. Some souls chose to explore far from that Unity... and, in the adventure, they forgot. Until in the midst of fear, an inner voice speaks to them again: the guide was always there.
    </p>
  </div>

  <div class="grid md:grid-cols-3 gap-6">
    <Card className="hover:bg-white/[0.08] transition-colors">
      <h3 class="text-xl font-serif font-bold text-dorado mb-3">The Origin</h3>
      <p class="text-texto-principal font-medium mb-2">A Light of love and unity.</p>
      <p class="text-sm text-texto-suave italic">It gives you back perspective.</p>
    </Card>

    <Card className="hover:bg-white/[0.08] transition-colors">
      <h3 class="text-xl font-serif font-bold text-dorado mb-3">The Forgetting</h3>
      <p class="text-texto-principal font-medium mb-2">Separation, confusion, fear.</p>
      <p class="text-sm text-texto-suave italic">It helps you name what you feel.</p>
    </Card>

    <Card className="hover:bg-white/[0.08] transition-colors">
      <h3 class="text-xl font-serif font-bold text-dorado mb-3">The Return</h3>
      <p class="text-texto-principal font-medium mb-2">An inner guide that never left.</p>
      <p class="text-sm text-texto-suave italic">It leaves you in peace.</p>
    </Card>
  </div>
</Section>
