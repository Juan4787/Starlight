<script lang="ts">
  import Section from '../ui/Section.svelte';
  import { slide } from 'svelte/transition';

  type FAQ = {
    question: string;
    answer: string;
    isOpen: boolean;
  };

  let faqs: FAQ[] = [
    {
      question: "Is it religious?",
      answer: "No. It speaks of God as love and inner guidance, without institutions or dogmas.",
      isOpen: false
    },
    {
      question: "What ages is it for?",
      answer: "It works for children (for its simplicity and symbolism) and for adults (for the message). Ideal to read together.",
      isOpen: false
    },
    {
      question: "How do I receive it?",
      answer: "In digital format (PDF), with immediate access after purchase.",
      isOpen: false
    },
    {
      question: "Can I print it?",
      answer: "Yes, you can print it for personal use.",
      isOpen: false
    },
    {
      question: "Is it worth paying for a digital story?",
      answer: "It is not just a story to read once. It is a reading you can reopen, share, and use as a ritual. If you seek quantity, this is not it. If you seek meaning, yes.",
      isOpen: false
    },
    {
      question: "How long is the reading?",
      answer: "It is short: perfect for a night ritual.",
      isOpen: false
    }
  ];

  const toggleFAQ = (index: number) => {
    faqs = faqs.map((faq, i) => ({
      ...faq,
      isOpen: i === index ? !faq.isOpen : false
    }));
  };
</script>

<Section id="faq">
  <div class="max-w-3xl mx-auto">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-serif font-bold mb-4 text-texto-principal">
        Frequently Asked Questions
      </h2>
    </div>

    <div class="space-y-4">
      {#each faqs as faq, i}
        <div class="bg-white/[0.04] border border-white/10 rounded-xl overflow-hidden transition-colors hover:bg-white/[0.06]">
          <button 
            class="w-full px-6 py-4 flex items-center justify-between text-left focus:outline-none"
            on:click={() => toggleFAQ(i)}
          >
            <span class="text-lg font-medium text-texto-principal">{faq.question}</span>
            <svg 
              class="w-5 h-5 text-dorado transition-transform duration-300 {faq.isOpen ? 'rotate-180' : ''}" 
              fill="none" 
              viewBox="0 0 24 24" 
              stroke="currentColor"
            >
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
            </svg>
          </button>
          
          {#if faq.isOpen}
            <div class="px-6 pb-4 text-texto-suave leading-relaxed" transition:slide>
              {faq.answer}
            </div>
          {/if}
        </div>
      {/each}
    </div>
  </div>
</Section>
