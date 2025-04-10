import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { motion } from "framer-motion";

export default function LegacyMemecoinPage() {
  return (
    <div className="min-h-screen bg-black text-white flex flex-col items-center justify-center px-6">
      <motion.h1
        initial={{ opacity: 0, y: -50 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 1 }}
        className="text-4xl md:text-6xl font-bold text-center mb-6"
      >
        Non vogliamo solo virali. Vogliamo leggenda.
      </motion.h1>

      <motion.p
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ delay: 0.5, duration: 1 }}
        className="text-lg md:text-xl text-center max-w-2xl mb-8"
      >
        Questa non è solo una coin. È un testamento. Un urlo nella blockchain: "Io c’ero".
        Non per il pump. Ma per lasciare un'impronta. Per quelli che si rifiutano di scomparire.
      </motion.p>

      <motion.div
        initial={{ opacity: 0, scale: 0.9 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ delay: 1, duration: 0.8 }}
        className="w-full max-w-md"
      >
        <Card className="bg-white/10 border-white/20 rounded-2xl shadow-lg">
          <CardContent className="p-6 text-center">
            <p className="text-xl font-semibold mb-4">
              Unisciti al patto. Diventa leggenda digitale.
            </p>
            <Button className="bg-white text-black font-bold text-lg px-8 py-4 rounded-xl">
              Entra nella community
            </Button>
          </CardContent>
        </Card>
      </motion.div>
    </div>
  );
}
