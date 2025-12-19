<script>
  import Navbar from '$lib/components/Navbar.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import ProblemSolution from '$lib/components/ProblemSolution.svelte';
  import Foundation from '$lib/components/Foundation.svelte';
  import FeatureSection from '$lib/components/FeatureSection.svelte';
  import FeatureVisual1 from '$lib/components/FeatureVisual1.svelte';
  import FeatureVisual2 from '$lib/components/FeatureVisual2.svelte';
  import FeatureVisual3 from '$lib/components/FeatureVisual3.svelte';
  import Testimonials from '$lib/components/Testimonials.svelte';
  import CTA from '$lib/components/CTA.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<Navbar />

<main>
  <Hero />
  <ProblemSolution />
  <Foundation />
  
  <FeatureSection
    align="right"
    colorClass="bg-[#fcd34d]"
    category="Control & visibility"
    title="Run your stack the way you wish it worked"
    description="Default gives you one place to see how everything works, and the power to change it without breaking anything."
    ctaText="Default for RevOps →"
    testimonial={{
        quote: "I don't just see Default as a Chili Piper replacement anymore. It's the control layer we're going to use to run GTM from...",
        author: "Matt McGonegle",
        role: "Director of GTM Operations",
        avatar: "https://api.dicebear.com/7.x/avataaars/svg?seed=Matt",
        readStory: true
    }}
    stats={[
        {value: "147", label: "tools consolidated under a single GTM control layer"},
        {value: "80+ rules", label: "routing rules defined once and reused across the GTM"},
        {value: "3", label: "systems replaced with one workflow engine"}
    ]}
  >
    <div slot="image" class="w-full h-full">
        <FeatureVisual1 />
    </div>
  </FeatureSection>

  <FeatureSection
    align="left"
    colorClass="bg-[#f472b6]"
    category="Connected foundation"
    title="Every tool speaks the same language"
    description="Default unifies every field and object around one shared data model, so your entire stack finally agrees on reality."
    ctaText="Platform overview →"
    testimonial={{
        quote: "Default replaced a clunky LeanData + Marketo + Salesforce setup in a workflow that we set up in just few hours.",
        author: "People Data Labs",
        role: "after using Default",
        avatar: "",
        readStory: true
    }}
  >
    <div slot="image" class="w-full h-full">
        <FeatureVisual2 />
    </div>
  </FeatureSection>

  <FeatureSection
    align="right"
    colorClass="bg-[#5850ec]"
    category="Revenue-grade execution"
    title="Stop losing leads you already paid for"
    description="Default automatically catches every qualified lead and ensures nothing gets dropped."
    ctaText="Default for Marketing →"
    testimonial={{
        quote: "Someone literally posted on Twitter wondering if the self-serve experience was hand-built. It wasn't—it was Default...",
        author: "Nick Lafferty",
        role: "Growth Marketing",
        avatar: "https://api.dicebear.com/7.x/avataaars/svg?seed=Nick",
        readStory: true
    }}
    stats={[
        {value: "3X", label: "higher inbound conversions"},
        {value: "140%", label: "increase in pipeline"},
        {value: "7 Days", label: "from demo to go-live"}
    ]}
  >
    <div slot="image" class="w-full h-full">
        <FeatureVisual3 />
    </div>
  </FeatureSection>

  <Testimonials />
  <CTA />
</main>

<Footer />

