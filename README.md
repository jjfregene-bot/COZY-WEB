export default function CozyCrochetWebsite() {
  return (
    <div className="min-h-screen bg-[#F5EFE6] text-[#2F4F4F] overflow-x-hidden">
      {/* NAVBAR */}
      <header className="w-full bg-[#F8F3EE] border-b border-[#E8DDD2] sticky top-0 z-50">
        <div className="max-w-7xl mx-auto px-6 lg:px-12 py-5 flex items-center justify-between">
          <div>
            <h1
              className="text-3xl leading-none"
              style={{ fontFamily: 'Playfair Display' }}
            >
              Explore
            </h1>
            <p className="uppercase text-[10px] tracking-[0.35em] mt-1 text-[#8B6B61]">
              Create • Connect • Protect
            </p>
          </div>

          <nav className="hidden md:flex gap-8 text-sm uppercase tracking-wide text-[#5A5A5A]">
            <a href="#" className="hover:text-[#C97C5D] transition-colors">Home</a>
            <a href="#" className="hover:text-[#C97C5D] transition-colors">Explore</a>
            <a href="#" className="hover:text-[#C97C5D] transition-colors">Create</a>
            <a href="#" className="hover:text-[#C97C5D] transition-colors">With Kids</a>
            <a href="#" className="hover:text-[#C97C5D] transition-colors">Cybersecurity</a>
            <a href="#" className="hover:text-[#C97C5D] transition-colors">Shop</a>
          </nav>
        </div>
      </header>

      {/* HERO */}
      <section className="relative px-6 lg:px-16 py-16 lg:py-24 bg-[#F8F3EE]">
        <div className="max-w-7xl mx-auto grid lg:grid-cols-2 gap-14 items-center">
          <div>
            <p className="uppercase tracking-[0.3em] text-xs text-[#8A756A] mb-5">
              Explore • Create • Connect • Protect
            </p>

            <h1
              className="text-5xl md:text-6xl leading-tight mb-8 text-[#2F4F4F]"
              style={{ fontFamily: 'Playfair Display' }}
            >
              A cozy space for exploration, creativity & digital confidence
            </h1>

            <p className="text-lg text-[#5B6767] leading-relaxed max-w-xl mb-10">
              I share inspiration for slower intentional living through travel, crochet, meaningful moments with children, and simple ways to stay safe online.
            </p>

            <div className="flex flex-wrap gap-5">
              <button className="bg-[#556B4F] text-white px-8 py-4 rounded-full shadow-lg hover:scale-105 transition-all duration-300">
                Explore The Blog
              </button>

              <button className="border border-[#D5C4B8] px-8 py-4 rounded-full bg-white hover:bg-[#EFE5DC] transition-all duration-300">
                Download Freebies
              </button>
            </div>
          </div>

          <div className="relative">
            <div className="rounded-[3rem] overflow-hidden shadow-2xl bg-white p-4 rotate-1">
              <div className="aspect-[4/3] rounded-[2.5rem] bg-gradient-to-br from-[#EAD7CE] via-[#F7F1EB] to-[#D9E5D5] flex items-center justify-center relative overflow-hidden">
                <div className="absolute top-12 left-12 text-7xl">🧶</div>
                <div className="absolute bottom-10 right-10 text-7xl">☕</div>
                <div className="text-center px-10 z-10">
                  <h2
                    className="text-4xl mb-5 text-[#5A504D]"
                    style={{ fontFamily: 'Playfair Display' }}
                  >
                    Slow Living
                  </h2>

                  <p className="text-[#6D6D6D] text-lg">
                    Creativity, mindfulness & safe digital living.
                  </p>
                </div>
              </div>
            </div>

            <div className="absolute -bottom-5 -left-5 bg-white rounded-3xl shadow-xl px-6 py-5 border border-[#E9DED4]">
              <p className="text-xs uppercase tracking-[0.25em] text-[#8A756A] mb-1">
                Featured Guide
              </p>
              <h3
                className="text-2xl"
                style={{ fontFamily: 'Playfair Display' }}
              >
                Cozy Crochet Starter Guide
              </h3>
            </div>
          </div>
        </div>
      </section>

      {/* CATEGORY GRID */}
      <section className="px-6 lg:px-16 py-20 bg-white">
        <div className="max-w-7xl mx-auto">
          <div className="text-center mb-16">
            <h2
              className="text-5xl mb-4 text-[#2F4F4F]"
              style={{ fontFamily: 'Playfair Display' }}
            >
              Explore all the things that matter
            </h2>

            <p className="text-[#6C7777] text-lg">
              A beautiful blend of creativity, calm living, learning & digital wellbeing.
            </p>
          </div>

          <div className="grid md:grid-cols-2 lg:grid-cols-5 gap-6">
            {[
              {
                icon: '🌍',
                title: 'Explore',
                text: 'Travel, hidden places & beautiful moments.'
              },
              {
                icon: '🍜',
                title: 'Food & Lifestyle',
                text: 'Comfort food, cafés & intentional living.'
              },
              {
                icon: '🧶',
                title: 'Knit & Crochet',
                text: 'Patterns, cozy creativity & slow hobbies.'
              },
              {
                icon: '👶',
                title: 'With Kids',
                text: 'Play-based learning & nurturing growth.'
              },
              {
                icon: '🔐',
                title: 'Cybersecurity',
                text: 'Simple online safety for everyday life.'
              }
            ].map((item, index) => (
              <div
                key={index}
                className="bg-[#F9F4EF] rounded-[2rem] p-8 shadow-sm hover:shadow-xl transition-all duration-300 border border-[#EFE4DA]"
              >
                <div className="text-5xl mb-6">{item.icon}</div>

                <h3
                  className="text-2xl mb-4 text-[#2F4F4F]"
                  style={{ fontFamily: 'Playfair Display' }}
                >
                  {item.title}
                </h3>

                <p className="text-[#6D7676] leading-relaxed text-sm">
                  {item.text}
                </p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* PRODUCT SECTION */}
      <section className="px-6 lg:px-16 py-24 bg-[#F8F3EE]">
        <div className="max-w-7xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
          <div className="bg-white rounded-[3rem] p-10 shadow-xl border border-[#ECE1D7]">
            <div className="aspect-[4/5] rounded-[2rem] bg-gradient-to-br from-[#DAB6A9] via-[#F8F3EE] to-[#D8E4D2] flex flex-col justify-center items-center text-center p-10">
              <div className="text-8xl mb-6">🧶</div>

              <h2
                className="text-4xl mb-4"
                style={{ fontFamily: 'Playfair Display' }}
              >
                Cozy Crochet Starter Guide
              </h2>

              <p className="text-[#6C7777] leading-relaxed max-w-sm">
                Beginner-friendly crochet guidance designed for calm intentional creativity.
              </p>
            </div>
          </div>

          <div>
            <p className="uppercase tracking-[0.3em] text-xs text-[#8A756A] mb-5">
              Featured Digital Product
            </p>

            <h2
              className="text-5xl leading-tight mb-8 text-[#2F4F4F]"
              style={{ fontFamily: 'Playfair Display' }}
            >
              Learn crochet slowly, confidently & beautifully
            </h2>

            <div className="space-y-5 mb-10 text-[#5F6969] text-lg">
              <p>✔ Essential tools & materials</p>
              <p>✔ Beginner-friendly stitches</p>
              <p>✔ Step-by-step mini project</p>
              <p>✔ Cozy printable PDF</p>
            </div>

            <button className="bg-[#1F2A44] text-white px-10 py-5 rounded-full shadow-xl hover:scale-105 transition-all duration-300">
              Get Your Guide — £9
            </button>
          </div>
        </div>
      </section>

      {/* CYBERSECURITY SECTION */}
      <section className="px-6 lg:px-16 py-24 bg-white">
        <div className="max-w-7xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
          <div>
            <p className="uppercase tracking-[0.3em] text-xs text-[#8A756A] mb-5">
              Digital Confidence Matters
            </p>

            <h2
              className="text-5xl leading-tight mb-8 text-[#2F4F4F]"
              style={{ fontFamily: 'Playfair Display' }}
            >
              Cybersecurity & Digital Wellness
            </h2>

            <p className="text-lg text-[#5F6969] leading-relaxed mb-8">
              Simple tips for a safer online life. Protect your privacy, your devices, and your peace of mind.
            </p>

            <div className="grid grid-cols-2 gap-5 mb-10">
              {[
                'Online Safety',
                'Privacy Awareness',
                'Scam Prevention',
                'Healthy Digital Habits'
              ].map((item, index) => (
                <div
                  key={index}
                  className="bg-[#F7F2EE] rounded-2xl p-5 border border-[#EFE5DB]"
                >
                  <p className="font-medium">🔐 {item}</p>
                </div>
              ))}
            </div>

            <button className="bg-[#556B4F] text-white px-10 py-5 rounded-full shadow-lg hover:scale-105 transition-all duration-300">
              Explore Cyber Tips
            </button>
          </div>

          <div className="rounded-[3rem] overflow-hidden shadow-2xl bg-gradient-to-br from-[#1F2A44] to-[#384B66] min-h-[500px] flex items-center justify-center text-white text-center p-12">
            <div>
              <div className="text-8xl mb-8">💻</div>
              <h3
                className="text-4xl mb-6"
                style={{ fontFamily: 'Playfair Display' }}
              >
                Stay Safe Online
              </h3>

              <p className="text-lg text-gray-200 leading-relaxed max-w-md mx-auto">
                Helping everyday people feel calm, informed, and protected in the digital world.
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* NEWSLETTER */}
      <section className="px-6 lg:px-16 py-24 bg-[#F8F3EE]">
        <div className="max-w-5xl mx-auto bg-[#1F2A44] rounded-[3rem] p-14 text-center text-white shadow-2xl">
          <p className="uppercase tracking-[0.35em] text-xs text-[#D8A7A7] mb-5">
            Stay Connected
          </p>

          <h2
            className="text-5xl leading-tight mb-8"
            style={{ fontFamily: 'Playfair Display' }}
          >
            Cozy inspiration delivered to your inbox
          </h2>

          <p className="text-lg text-gray-300 max-w-2xl mx-auto leading-relaxed mb-10">
            Get crochet inspiration, cozy lifestyle ideas, educational tips & simple cybersecurity reminders.
          </p>

          <div className="flex flex-col md:flex-row gap-5 max-w-2xl mx-auto">
            <input
              type="email"
              placeholder="Your email address"
              className="flex-1 px-6 py-5 rounded-full text-black outline-none"
            />

            <button className="bg-[#D8A7A7] text-[#1F2A44] px-10 py-5 rounded-full font-semibold hover:scale-105 transition-all duration-300">
              Yes, Please!
            </button>
          </div>
        </div>
      </section>

      {/* FOOTER */}
      <footer className="bg-white py-10 text-center border-t border-[#EEE3D9]">
        <p className="text-[#6C7777] text-sm">
          © 2026 Explore • Create • Connect • Protect
        </p>
      </footer>
    </div>
  );
}
