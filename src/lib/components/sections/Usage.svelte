<script lang="ts">
  import Section from '../ui/Section.svelte';
  import Card from '../ui/Card.svelte';
</script>

<Section>
  <div class="text-center mb-16">
    <h2 class="text-3xl md:text-4xl font-serif font-bold mb-6 text-texto-principal">
      3 simple ways to experience it
    </h2>
  </div>

  <div class="grid md:grid-cols-3 gap-6">
    <Card className="text-center group hover:-translate-y-2 transition-transform duration-300">
      <div class="w-16 h-16 mx-auto mb-6 rounded-full bg-dorado/10 flex items-center justify-center text-3xl group-hover:scale-110 transition-transform">
        🌙
      </div>
      <h3 class="text-xl font-serif font-bold text-texto-principal mb-3">Night ritual</h3>
      <p class="text-texto-suave mb-4 text-sm uppercase tracking-wider opacity-60">7–12 min</p>
      <p class="text-texto-suave italic">A reading, a question, a hug. Ideal to wind down before sleeping.</p>
    </Card>

    <Card className="text-center group hover:-translate-y-2 transition-transform duration-300">
      <div class="w-16 h-16 mx-auto mb-6 rounded-full bg-dorado/10 flex items-center justify-center text-3xl group-hover:scale-110 transition-transform">
        🧘‍♀️
      </div>
      <h3 class="text-xl font-serif font-bold text-texto-principal mb-3">Reading for adults</h3>
      <p class="text-texto-suave mb-4 text-sm uppercase tracking-wider opacity-60">Introspection</p>
      <p class="text-texto-suave italic">As a personal reminder: "come home". To read in silence when you need peace.</p>
    </Card>

    <Card className="text-center group hover:-translate-y-2 transition-transform duration-300">
      <div class="w-16 h-16 mx-auto mb-6 rounded-full bg-dorado/10 flex items-center justify-center text-3xl group-hover:scale-110 transition-transform">
        👨‍👩‍👧‍👦
      </div>
      <h3 class="text-xl font-serif font-bold text-texto-principal mb-3">Shared moment</h3>
      <p class="text-texto-suave mb-4 text-sm uppercase tracking-wider opacity-60">Connection</p>
      <p class="text-texto-suave italic">To converse without imposing, just opening the space for deep questions.</p>
    </Card>
  </div>
</Section>
