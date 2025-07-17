import React from "react"; import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button";

export default function ZubaanAIHome() { return ( <div className="min-h-screen bg-gradient-to-b from-white to-orange-50 p-6 text-center"> <h1 className="text-4xl font-bold text-orange-600 mb-4">Zubaan AI</h1> <p className="text-lg text-gray-700 mb-6"> Real-time Voice Assistant that Converts Hindi to Indian Regional Languages. </p>

<div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4 max-w-4xl mx-auto">
    {["Marathi", "Bhojpuri", "Tamil", "Gujarati", "Bengali"].map((lang) => (
      <Card key={lang} className="shadow-md">
        <CardContent className="p-4">
          <h2 className="text-xl font-semibold text-orange-500">{lang}</h2>
          <p className="text-sm text-gray-600 mt-2">
            Speak in Hindi and hear in {lang} instantly.
          </p>
        </CardContent>
      </Card>
    ))}
  </div>

  <div className="mt-8">
    <Button className="bg-orange-500 hover:bg-orange-600 text-white px-6 py-2 rounded-2xl shadow">
      Try Demo (Coming Soon)
    </Button>
  </div>

  <footer className="mt-12 text-sm text-gray-500">
    Built by Sagar Raj | REC College | © 2025 Zubaan AI
  </footer>
</div>

); }

# Zuban-AI
