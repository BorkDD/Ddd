import { Button } from "@/components/ui/button"
import { Card, CardContent } from "@/components/ui/card"
import { RocketIcon, PizzaIcon, WalletIcon } from "lucide-react"
import { motion } from "framer-motion"

export default function LandingPage() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-black via-zinc-900 to-gray-800 text-white p-6">
      <div className="max-w-5xl mx-auto grid gap-10">
        {/* Hero Section */}
        <motion.div
          initial={{ opacity: 0, y: -30 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.8 }}
          className="text-center space-y-6"
        >
          <h1 className="text-5xl font-extrabold text-white">
            DD — Decentralized Delivery
          </h1>
          <p className="text-xl text-zinc-400 max-w-2xl mx-auto">
            Первая в мире Web3-доставка еды в реальном времени. Курьер в мегаполисе. Стрим. Токен. И немного пиццы.
          </p>
          <Button className="text-lg px-6 py-3 rounded-2xl text-black bg-green-400 hover:bg-green-300">
            🚀 Запустить $DD на pump.fun
          </Button>
        </motion.div>

        {/* Features */}
        <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
          <Card className="bg-zinc-800 text-white">
            <CardContent className="p-6 space-y-4">
              <PizzaIcon className="w-10 h-10 text-yellow-400" />
              <h3 className="text-xl font-semibold">🍕 IRL-Доставка</h3>
              <p className="text-zinc-400">Реальный курьер. Настоящие миссии. Еда, стрим и вызовы от комьюнити.</p>
            </CardContent>
          </Card>
          <Card className="bg-zinc-800 text-white">
            <CardContent className="p-6 space-y-4">
              <WalletIcon className="w-10 h-10 text-purple-400" />
              <h3 className="text-xl font-semibold">💸 $DD Токен</h3>
              <p className="text-zinc-400">Запущен на Solana через pump.fun. Владей, участвуй, влияй на сюжет IRL.</p>
            </CardContent>
          </Card>
          <Card className="bg-zinc-800 text-white">
            <CardContent className="p-6 space-y-4">
              <RocketIcon className="w-10 h-10 text-cyan-400" />
              <h3 className="text-xl font-semibold">📡 Стримы</h3>
              <p className="text-zinc-400">Смотри, как Web3 выходит на улицы. TikTok, Telegram, YouTube — выбирай свой фронт.</p>
            </CardContent>
          </Card>
        </div>

        {/* Call to action */}
        <motion.div
          initial={{ opacity: 0, y: 30 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ delay: 0.4, duration: 0.8 }}
          className="text-center space-y-4"
        >
          <h2 className="text-3xl font-bold">Готов стать частью DD-миссии?</h2>
          <p className="text-zinc-400">Зайди в Telegram, следи за стримами и держи $DD, чтобы менять маршрут доставки в реальном времени.</p>
          <Button className="bg-white text-black px-6 py-3 rounded-2xl hover:bg-zinc-200">
            💬 Вступить в Telegram
          </Button>
        </motion.div>
      </div>
    </div>
  )
}# Ddd
