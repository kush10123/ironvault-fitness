import { useState } from "react";
import {
  Dumbbell,
  ShoppingCart,
  Phone,
  Mail,
  MapPin,
  ArrowRight,
  Star,
  ShieldCheck,
} from "lucide-react";

import { motion } from "framer-motion";

const products = [
  {
    id: 1,
    name: "Elite Treadmill X9",
    price: "$2,400",
    image:
      "https://images.unsplash.com/photo-1576678927484-cc907957088c?q=80&w=1200&auto=format&fit=crop",
  },
  {
    id: 2,
    name: "Pro Bench Press",
    price: "$1,200",
    image:
      "https://images.unsplash.com/photo-1598289431512-b97b0917affc?q=80&w=1200&auto=format&fit=crop",
  },
  {
    id: 3,
    name: "Adjustable Dumbbells",
    price: "$450",
    image:
      "https://images.unsplash.com/photo-1583454110551-21f2fa2afe61?q=80&w=1200&auto=format&fit=crop",
  },
];

export default function MasonryServiceLLC() {
  const [cart, setCart] = useState(0);

  return (
    <div className="bg-black text-white min-h-screen">
      {/* NAVBAR */}
      <nav className="flex justify-between items-center px-6 md:px-16 py-6 border-b border-white/10 backdrop-blur-lg sticky top-0 bg-black/70 z-50">
        <div>
          <h1 className="text-2xl font-bold tracking-wide">
            Masonry Service LLC
          </h1>
          <p className="text-sm text-gray-400">
            Gym Equipment Marketplace
          </p>
        </div>

        <div className="flex items-center gap-6">
          <button className="relative">
            <ShoppingCart />

            <span className="absolute -top-2 -right-2 bg-red-500 text-xs px-2 rounded-full">
              {cart}
            </span>
          </button>
        </div>
      </nav>

      {/* HERO SECTION */}
      <section className="grid md:grid-cols-2 gap-10 items-center px-6 md:px-16 py-20">
        <motion.div
          initial={{ opacity: 0, y: 30 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.8 }}
        >
          <div className="inline-flex items-center gap-2 bg-white/10 border border-white/10 px-4 py-2 rounded-full mb-6">
            <Dumbbell size={18} />
            <span>Premium USA Gym Equipment</span>
          </div>

          <h2 className="text-5xl md:text-7xl font-black leading-tight mb-6">
            Buy & Sell
            <span className="text-red-500"> Gym Equipment</span>
          </h2>

          <p className="text-gray-400 text-lg mb-8 leading-relaxed">
            Masonry Service LLC helps commercial gyms, fitness studios,
            and home gym owners buy, sell, and trade premium fitness
            equipment.
          </p>

          <div className="flex flex-wrap gap-4">
            <button className="bg-red-500 hover:bg-red-600 transition px-8 py-4 rounded-2xl font-semibold flex items-center gap-2 shadow-lg shadow-red-500/20">
              Browse Equipment
              <ArrowRight size={18} />
            </button>

            <button className="border border-white/20 hover:bg-white/10 transition px-8 py-4 rounded-2xl font-semibold">
              Sell Your Equipment
            </button>
          </div>
        </motion.div>

        <motion.div
          initial={{ opacity: 0, scale: 0.9 }}
          animate={{ opacity: 1, scale: 1 }}
          transition={{ duration: 0.8 }}
          className="relative"
        >
          <img
            src="https://images.unsplash.com/photo-1534438327276-14e5300c3a48?q=80&w=1200&auto=format&fit=crop"
            alt="Gym Equipment"
            className="rounded-3xl shadow-2xl h-[500px] object-cover w-full"
          />

          <div className="absolute -bottom-6 -left-6 bg-white text-black rounded-2xl p-5 shadow-2xl w-64">
            <div className="flex items-center gap-2 mb-2">
              {[...Array(5)].map((_, i) => (
                <Star
                  key={i}
                  className="text-yellow-500 fill-yellow-500"
                  size={18}
                />
              ))}
            </div>

            <p className="font-bold text-lg">
              Trusted USA Supplier
            </p>

            <p className="text-sm text-gray-600">
              Commercial & Home Gym Solutions
            </p>
          </div>
        </motion.div>
      </section>

      {/* FEATURES */}
      <section className="grid md:grid-cols-3 gap-6 px-6 md:px-16 py-10">
        <div className="bg-white/5 border border-white/10 rounded-3xl p-8 hover:bg-white/10 transition">
          <ShieldCheck
            className="text-red-500 mb-4"
            size={40}
          />

          <h3 className="text-2xl font-bold mb-3">
            Trusted Trading
          </h3>

          <p className="text-gray-400">
            Safe and verified equipment transactions for commercial and
            personal gyms.
          </p>
        </div>

        <div className="bg-white/5 border border-white/10 rounded-3xl p-8 hover:bg-white/10 transition">
          <Dumbbell className="text-red-500 mb-4" size={40} />

          <h3 className="text-2xl font-bold mb-3">
            Premium Equipment
          </h3>

          <p className="text-gray-400">
            High-quality treadmills, benches, dumbbells, cardio
            machines and more.
          </p>
        </div>

        <div className="bg-white/5 border border-white/10 rounded-3xl p-8 hover:bg-white/10 transition">
          <ShoppingCart
            className="text-red-500 mb-4"
            size={40}
          />

          <h3 className="text-2xl font-bold mb-3">
            Fast Ordering
          </h3>

          <p className="text-gray-400">
            Modern ecommerce experience with fast checkout and easy
            ordering.
          </p>
        </div>
      </section>

      {/* PRODUCTS */}
      <section className="px-6 md:px-16 py-20">
        <div className="flex justify-between items-center mb-10">
          <div>
            <h2 className="text-4xl font-black">
              Featured Equipment
            </h2>

            <p className="text-gray-400 mt-2">
              Top fitness machines & strength equipment
            </p>
          </div>
        </div>

        <div className="grid md:grid-cols-3 gap-8">
          {products.map((product) => (
            <motion.div
              whileHover={{ y: -8 }}
              key={product.id}
              className="bg-white/5 border border-white/10 rounded-3xl overflow-hidden shadow-xl"
            >
              <img
                src={product.image}
                alt={product.name}
                className="h-72 w-full object-cover"
              />

              <div className="p-6">
                <h3 className="text-2xl font-bold mb-2">
                  {product.name}
                </h3>

                <p className="text-red-500 text-xl font-semibold mb-5">
                  {product.price}
                </p>

                <button
                  onClick={() => setCart(cart + 1)}
                  className="w-full bg-red-500 hover:bg-red-600 transition py-4 rounded-2xl font-semibold"
                >
                  Add To Cart
                </button>
              </div>
            </motion.div>
          ))}
        </div>
      </section>

      {/* CONTACT */}
      <section className="px-6 md:px-16 py-20">
        <div className="bg-gradient-to-r from-red-600 to-red-500 rounded-[40px] p-10 md:p-16 shadow-2xl">
          <h2 className="text-5xl font-black mb-6">
            Contact Masonry Service LLC
          </h2>

          <div className="grid md:grid-cols-2 gap-10 text-lg">
            <div className="space-y-5">
              <div className="flex items-center gap-3">
                <Phone />
                <span>8707846164</span>
              </div>

              <div className="flex items-center gap-3">
                <Mail />
                <span>ervinanthony86@gmail.com</span>
              </div>

              <div className="flex items-center gap-3">
                <MapPin />
                <span>
                  5203 SW Villa Street, Bentonville, Arkansas,
                  72712
                </span>
              </div>
            </div>

            <div>
              <h3 className="text-3xl font-bold mb-3">CEO</h3>

              <p className="text-xl">Anthony Ervin</p>
            </div>
          </div>
        </div>
      </section>

      {/* FOOTER */}
      <footer className="border-t border-white/10 px-6 md:px-16 py-8 text-gray-500 text-center">
        © 2026 Masonry Service LLC — All Rights Reserved.
      </footer>
    </div>
  );
}
