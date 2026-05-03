# me
hi there, i'm gladys.
i'm a growth manager at rednote, a social media platform with 300M MAU and i focus on scale it globally.
my background sits at the intersection of building and investing
before rednote, i operated as a founder-investor hybrid, building an incubator in palo alto
i'm deeply committed to the tech ecosystem and am always looking to connect with builders, investors, and creators in the SF/Bay Area and beyond


import React from "react";
import { motion } from "framer-motion";
import {
  ArrowRight,
  Mail,
  Instagram,
  Linkedin,
  ExternalLink,
  ImagePlus,
} from "lucide-react";

const EVENT_PLACEHOLDERS = [
  "Founder Mixers",
  "Investors Dinners",
  "Campus Events",
  "Creator Summit",
];

const fadeInUp = {
  hidden: { opacity: 0, y: 20 },
  visible: {
    opacity: 1,
    y: 0,
    transition: { duration: 0.6, ease: [0.16, 1, 0.3, 1] },
  },
};

const staggerContainer = {
  hidden: { opacity: 0 },
  visible: {
    opacity: 1,
    transition: {
      staggerChildren: 0.1,
    },
  },
};

export default function Home() {
  return (
    <div className="min-h-screen bg-background text-foreground selection:bg-primary selection:text-primary-foreground font-sans">
      {/* 1. NAV */}
      <nav className="fixed top-0 w-full z-50 bg-background/80 backdrop-blur-md border-b border-border/40">
        <div className="max-w-7xl mx-auto px-6 h-16 flex items-center justify-between">
          <div className="font-serif font-bold text-lg tracking-tight">
            Gladys Wan
          </div>
          <a
            href="#connect"
            className="text-sm font-medium text-muted-foreground hover:text-foreground transition-colors flex items-center gap-2"
          >
            Let's connect <ArrowRight className="w-4 h-4" />
          </a>
        </div>
      </nav>

      {/* 2. HERO */}
      <section className="pt-40 pb-24 px-6 md:pt-48 md:pb-32 flex flex-col justify-center max-w-7xl mx-auto">
        <motion.div
          initial="hidden"
          animate="visible"
          variants={staggerContainer}
          className="max-w-4xl"
        >
          <motion.div
            variants={fadeInUp}
            className="mb-6 flex flex-wrap items-center gap-3"
          >
            <span className="px-3 py-1 bg-secondary text-secondary-foreground rounded-full text-xs font-medium tracking-wide border border-border/50">
              Growth @ rednote
            </span>
            <span className="px-3 py-1 bg-secondary text-secondary-foreground rounded-full text-xs font-medium tracking-wide border border-border/50">
              Bay Area
            </span>
          </motion.div>

          <motion.h1
            variants={fadeInUp}
            className="text-6xl md:text-8xl lg:text-9xl font-serif font-bold leading-[1.1] tracking-tight mb-8 text-foreground"
          >
            Gladys Wan
          </motion.h1>

          <motion.p
            variants={fadeInUp}
            className="text-xl md:text-2xl text-muted-foreground max-w-2xl leading-relaxed mb-12"
          >
            Building rednote's US presence from scratch. I bring founders, VCs,
            creators, and students together to build lasting communities.
          </motion.p>

          <motion.div
            variants={fadeInUp}
            className="grid grid-cols-2 md:grid-cols-4 gap-6 py-8 border-y border-border/40"
          >
            <div>
              <div className="text-3xl font-serif font-bold text-foreground">
                89
              </div>
              <div className="text-sm text-muted-foreground mt-1">
                Events Hosted
              </div>
            </div>
            <div>
              <div className="text-3xl font-serif font-bold text-foreground">
                100+
              </div>
              <div className="text-sm text-muted-foreground mt-1">
                Bay Area Events
              </div>
            </div>
            <div>
              <div className="text-3xl font-serif font-bold text-foreground">
                1st
              </div>
              <div className="text-sm text-muted-foreground mt-1">
                US Hire @ rednote
              </div>
            </div>
            <div>
              <div className="text-3xl font-serif font-bold text-foreground">
                SF
              </div>
              <div className="text-sm text-muted-foreground mt-1">Based</div>
            </div>
          </motion.div>
        </motion.div>
      </section>

      {/* 3. ABOUT */}
      <section className="py-24 px-6 bg-secondary/30">
        <motion.div
          initial="hidden"
          whileInView="visible"
          viewport={{ once: true, margin: "-100px" }}
          variants={staggerContainer}
          className="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-16 items-start"
        >
          <motion.div variants={fadeInUp}>
            <h2 className="text-3xl md:text-4xl font-serif font-bold mb-6">
              Connecting the right people.
            </h2>
            <div className="space-y-6 text-muted-foreground text-lg leading-relaxed">
              <p>
                As the first US hire at rednote, I'm building our American
                presence from the ground up. My focus is on strategic growth,
                partnering with creators, students, and early-stage founders to
                establish a foothold in a competitive market.
              </p>
              <p>
                Before rednote, I cut my teeth producing 100+ events across the
                Bay Area—from intimate founder dinners to massive tech mixers. I
                know how to curate a room, drive engagement, and turn a
                gathering into a movement.
              </p>
            </div>
          </motion.div>
          <motion.div
            variants={fadeInUp}
            className="bg-card border border-border p-8 rounded-2xl"
          >
            <h3 className="font-serif font-bold text-xl mb-6">
              Who I work with
            </h3>
            <ul className="space-y-4">
              <li className="flex items-start gap-4">
                <div className="w-1.5 h-1.5 rounded-full bg-primary mt-2"></div>
                <div>
                  <div className="font-bold text-foreground">
                    Founders & VCs
                  </div>
                  <div className="text-sm text-muted-foreground">
                    Curating high-signal environments for deal-making and
                    partnerships.
                  </div>
                </div>
              </li>
              <li className="flex items-start gap-4">
                <div className="w-1.5 h-1.5 rounded-full bg-primary mt-2"></div>
                <div>
                  <div className="font-bold text-foreground">Creators</div>
                  <div className="text-sm text-muted-foreground">
                    Scaling rednote's creator ecosystem in the US.
                  </div>
                </div>
              </li>
              <li className="flex items-start gap-4">
                <div className="w-1.5 h-1.5 rounded-full bg-primary mt-2"></div>
                <div>
                  <div className="font-bold text-foreground">Students</div>
                  <div className="text-sm text-muted-foreground">
                    Building grassroots brand awareness at top universities.
                  </div>
                </div>
              </li>
            </ul>
          </motion.div>
        </motion.div>
      </section>

      {/* 4. EVENTS GALLERY */}
      <section className="py-32 px-6 max-w-7xl mx-auto">
        <motion.div
          initial="hidden"
          whileInView="visible"
          viewport={{ once: true, margin: "-100px" }}
          variants={staggerContainer}
          className="mb-16 flex flex-col md:flex-row md:items-end justify-between gap-6"
        >
          <div>
            <motion.h2
              variants={fadeInUp}
              className="text-4xl md:text-5xl font-serif font-bold mb-4"
            >
              The Work
            </motion.h2>
            <motion.p
              variants={fadeInUp}
              className="text-xl text-muted-foreground"
            >
              89 events hosted. 49 attended.
            </motion.p>
          </div>
          <motion.a
            variants={fadeInUp}
            href="https://luma.com/user/gladyswan4"
            target="_blank"
            rel="noreferrer"
            className="inline-flex items-center gap-2 text-primary hover:text-primary/80 transition-colors font-medium"
          >
            View on Luma <ExternalLink className="w-4 h-4" />
          </motion.a>
        </motion.div>

        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
          {EVENT_PLACEHOLDERS.map((label, i) => (
            <motion.div
              key={label}
              initial={{ opacity: 0, y: 20 }}
              whileInView={{ opacity: 1, y: 0 }}
              transition={{ delay: i * 0.07 }}
              viewport={{ once: true }}
              className="group relative aspect-[4/3] overflow-hidden rounded-xl bg-secondary/40 border border-border/50 hover:border-primary/40 transition-colors duration-300 flex flex-col items-center justify-center gap-3"
            >
              <ImagePlus className="w-8 h-8 text-muted-foreground/40 group-hover:text-primary/50 transition-colors duration-300" />
              <span className="text-sm font-medium text-muted-foreground/60 group-hover:text-muted-foreground transition-colors duration-300">
                {label}
              </span>
            </motion.div>
          ))}
        </div>
      </section>

      {/* 5. EXPERIENCE */}
      <section className="py-24 px-6 bg-secondary/20 border-y border-border/40">
        <motion.div
          initial="hidden"
          whileInView="visible"
          viewport={{ once: true, margin: "-100px" }}
          variants={staggerContainer}
          className="max-w-4xl mx-auto"
        >
          <motion.h2
            variants={fadeInUp}
            className="text-3xl md:text-4xl font-serif font-bold mb-16"
          >
            Experience
          </motion.h2>

          <div className="space-y-12">
            <motion.div variants={fadeInUp} className="relative pl-8 md:pl-0">
              <div className="md:grid md:grid-cols-[1fr_3fr] gap-8">
                <div className="mb-2 md:mb-0 md:text-right mt-1">
                  <div className="text-primary font-bold text-sm tracking-wide uppercase">
                    Current
                  </div>
                </div>
                <div className="relative">
                  <div className="hidden md:block absolute -left-[29px] top-1.5 w-3 h-3 rounded-full bg-primary ring-4 ring-background" />
                  <h3 className="text-2xl font-serif font-bold text-foreground">
                    Growth Manager
                  </h3>
                  <div className="text-muted-foreground font-medium mb-4">
                    rednote
                  </div>
                  <p className="text-muted-foreground leading-relaxed">
                    First US hire. Leading community-led growth strategies to
                    build rednote's presence in America. Spearheading lifestyle,
                    creator, and tech events that drive strategic user
                    acquisition.
                  </p>
                </div>
              </div>
            </motion.div>

            <motion.div variants={fadeInUp} className="relative pl-8 md:pl-0">
              <div className="md:grid md:grid-cols-[1fr_3fr] gap-8">
                <div className="mb-2 md:mb-0 md:text-right mt-1">
                  <div className="text-muted-foreground font-bold text-sm tracking-wide uppercase">
                    Previous
                  </div>
                </div>
                <div className="relative">
                  <div className="hidden md:block absolute -left-[29px] top-1.5 w-3 h-3 rounded-full bg-border ring-4 ring-background" />
                  <h3 className="text-2xl font-serif font-bold text-foreground">
                    Community & Partnerships
                  </h3>
                  <div className="text-muted-foreground font-medium mb-4">
                    Beta University / Bay Area Events
                  </div>
                  <p className="text-muted-foreground leading-relaxed">
                    Produced over 100 bespoke events ranging from intimate
                    founder dinners to large-scale venture capital summits.
                    Owned end-to-end execution, guest curation, and partnership
                    development across the Bay Area startup ecosystem.
                  </p>
                </div>
              </div>
            </motion.div>
          </div>
        </motion.div>
      </section>

      {/* GTM / BRAND PARTNERS */}
      <section className="py-24 px-6 border-t border-border/40">
        <motion.div
          initial="hidden"
          whileInView="visible"
          viewport={{ once: true, margin: "-80px" }}
          variants={staggerContainer}
          className="max-w-5xl mx-auto"
        >
          <motion.div
            variants={fadeInUp}
            className="mb-4 flex items-center gap-3"
          >
            <div className="h-[1px] w-8 bg-primary/60" />
            <span className="text-xs font-semibold uppercase tracking-widest text-primary/80">
              GTM & Sales Engine
            </span>
          </motion.div>
          <motion.h2
            variants={fadeInUp}
            className="text-3xl md:text-4xl font-serif font-bold mb-4"
          >
            Events as pipeline.
          </motion.h2>
          <motion.p
            variants={fadeInUp}
            className="text-lg text-muted-foreground mb-16 max-w-2xl"
          >
            I partner with growth-stage and enterprise companies to turn events
            into a high-converting GTM channel — driving qualified pipeline,
            brand credibility, and strategic relationships.
          </motion.p>

          <motion.div
            variants={fadeInUp}
            className="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-6 gap-3"
          >
            {[
              { name: "Nebius", tag: "AI Cloud" },
              { name: "UCloud", tag: "NASDAQ: UCL" },
              { name: "Carta", tag: "FinTech" },
              { name: "Fidelity", tag: "Finance" },
              { name: "DevRev", tag: "Dev Tools" },
              { name: "+ more", tag: "" },
            ].map(({ name, tag }) => (
              <div
                key={name}
                className="flex flex-col items-center justify-center gap-1 py-6 px-4 rounded-xl bg-secondary/40 border border-border/50 hover:border-primary/40 hover:bg-secondary/60 transition-all duration-300"
              >
                <span className="font-bold text-foreground text-sm text-center">
                  {name}
                </span>
                {tag && (
                  <span className="text-xs text-muted-foreground/70 text-center">
                    {tag}
                  </span>
                )}
              </div>
            ))}
          </motion.div>

          <motion.p
            variants={fadeInUp}
            className="mt-10 text-sm text-muted-foreground/60 max-w-xl"
          >
            From intimate founder dinners to 500-person mixers — I design events
            that create real business outcomes for partners, not just headcount.
          </motion.p>
        </motion.div>
      </section>

      {/* 6. CONNECT */}
      <section
        id="connect"
        className="py-32 px-6 max-w-7xl mx-auto text-center"
      >
        <motion.div
          initial="hidden"
          whileInView="visible"
          viewport={{ once: true }}
          variants={staggerContainer}
          className="max-w-2xl mx-auto"
        >
          <motion.img
            variants={fadeInUp}
            src="https://images.lumacdn.com/cdn-cgi/image/format=auto,fit=cover,dpr=2,anim=false,background=white,quality=75,width=400,height=400/avatars/ky/7043eab9-f862-4738-8fbd-68fa990264e3"
            alt="Gladys Wan"
            className="w-24 h-24 rounded-full mx-auto mb-8 border-4 border-card object-cover"
          />
          <motion.h2
            variants={fadeInUp}
            className="text-5xl md:text-7xl font-serif font-bold mb-6"
          >
            Let's work together.
          </motion.h2>
          <motion.p
            variants={fadeInUp}
            className="text-xl text-muted-foreground mb-12"
          >
            Looking to collaborate, host an event, or talk growth? Reach out.
          </motion.p>

          <motion.div
            variants={fadeInUp}
            className="flex flex-col sm:flex-row items-center justify-center gap-4"
          >
            <a
              href="mailto:hello@example.com"
              className="w-full sm:w-auto inline-flex items-center justify-center gap-2 bg-primary text-primary-foreground px-6 py-3 rounded-lg font-medium hover:bg-primary/90 transition-colors"
            >
              <Mail className="w-4 h-4" /> Email me
            </a>
            <a
              href="https://www.linkedin.com/in/gladyswan"
              target="_blank"
              rel="noreferrer"
              className="w-full sm:w-auto inline-flex items-center justify-center gap-2 px-6 py-3 rounded-lg font-medium border border-border hover:bg-secondary transition-colors"
            >
              <Linkedin className="w-4 h-4" /> LinkedIn
            </a>
            <a
              href="https://instagram.com/gladyswan4"
              target="_blank"
              rel="noreferrer"
              className="w-full sm:w-auto inline-flex items-center justify-center gap-2 px-6 py-3 rounded-lg font-medium border border-border hover:bg-secondary transition-colors"
            >
              <Instagram className="w-4 h-4" /> Instagram
            </a>
          </motion.div>
        </motion.div>
      </section>

      <footer className="py-8 px-6 text-center border-t border-border/40 text-sm text-muted-foreground flex flex-col sm:flex-row items-center justify-center gap-4">
        <span>
          &copy; {new Date().getFullYear()} Gladys Wan. All rights reserved.
        </span>
      </footer>
    </div>
  );
}
