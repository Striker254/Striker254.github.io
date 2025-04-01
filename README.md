import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { motion } from "framer-motion";

const FootballGameSite = () => {
  return (
    <div className="min-h-screen bg-gray-900 text-white p-4">
      <header className="text-center text-4xl font-bold p-6">Football Live</header>
      <main className="grid grid-cols-1 md:grid-cols-3 gap-6">
        <Card className="bg-gray-800 p-4 rounded-2xl shadow-lg">
          <CardContent>
            <h2 className="text-2xl font-semibold">Live Matches</h2>
            <p className="text-gray-400">Watch ongoing games in real-time.</p>
            <Button className="mt-4 bg-green-600 w-full">Watch Now</Button>
          </CardContent>
        </Card>

        <Card className="bg-gray-800 p-4 rounded-2xl shadow-lg">
          <CardContent>
            <h2 className="text-2xl font-semibold">Upcoming Fixtures</h2>
            <p className="text-gray-400">Check out the schedule of upcoming matches.</p>
            <Button className="mt-4 bg-blue-600 w-full">View Fixtures</Button>
          </CardContent>
        </Card>

        <Card className="bg-gray-800 p-4 rounded-2xl shadow-lg">
          <CardContent>
            <h2 className="text-2xl font-semibold">Match Highlights</h2>
            <p className="text-gray-400">Catch up on the best moments.</p>
            <Button className="mt-4 bg-red-600 w-full">Watch Highlights</Button>
          </CardContent>
        </Card>
      </main>
    </div>
  );
};

export default FootballGameSite;
