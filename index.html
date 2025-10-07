import React, { useState } from 'react';
import { LineChart, Line, XAxis, YAxis, CartesianGrid, Tooltip, Legend, ReferenceLine, Area, AreaChart } from 'recharts';

const BacchicEngine = () => {
  const [activeView, setActiveView] = useState('overview');
  const [reservoirLevel, setReservoirLevel] = useState(0);
  const [isRitual, setIsRitual] = useState(false);
  const [cyclePhase, setCyclePhase] = useState(0);

  // Generate data for reservoir accumulation
  const generateReservoirData = () => {
    const data = [];
    let epsilon = 0;
    for (let day = 0; day <= 30; day++) {
      if (day % 7 === 0 && day > 0) {
        // Ritual discharge every 7 days
        epsilon = epsilon * 0.2; // Discharge to 20%
      } else {
        epsilon += 0.5 + Math.random() * 0.3; // Daily accumulation
      }
      data.push({
        day,
        epsilon: epsilon,
        threshold: 8,
        danger: 12,
        ritual: day % 7 === 0 && day > 0 ? epsilon : null
      });
    }
    return data;
  };

  // Generate data for pathological accumulation (no rituals)
  const generatePathologicalData = () => {
    const data = [];
    let epsilon = 0;
    for (let day = 0; day <= 30; day++) {
      epsilon += 0.5 + Math.random() * 0.3;
      data.push({
        day,
        epsilon: epsilon,
        threshold: 8,
        danger: 12
      });
    }
    return data;
  };

  // Phase diagram data
  const phaseData = [
    { phase: 'θ′ Soil', value: 2, color: '#8B4513', description: 'Raw variance accumulates' },
    { phase: 'θ Roots', value: 4, color: '#CD853F', description: 'Energy encodes into ritual' },
    { phase: 'Σ Trunk', value: 7, color: '#DEB887', description: 'Compression into rhythm' },
    { phase: 'h(t) Branch', value: 9, color: '#FF6347', description: 'Explosive release' },
    { phase: 'ΔS Canopy', value: 3, color: '#4169E1', description: 'Integration & ledger' }
  ];

  const reservoirData = generateReservoirData();
  const pathologicalData = generatePathologicalData();

  return (
    <div className="w-full max-w-6xl mx-auto p-6 bg-slate-900 text-slate-100 min-h-screen">
      <div className="mb-8">
        <h1 className="text-4xl font-bold mb-2 bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">
          The Bacchic Engine
        </h1>
        <p className="text-slate-400 text-lg">Thermodynamic Control System for ε Accumulation</p>
      </div>

      {/* Navigation */}
      <div className="flex gap-2 mb-6 flex-wrap">
        {['overview', 'reservoir', 'failure', 'phases', 'application'].map(view => (
          <button
            key={view}
            onClick={() => setActiveView(view)}
            className={`px-4 py-2 rounded-lg transition-all ${
              activeView === view 
                ? 'bg-purple-600 text-white' 
                : 'bg-slate-800 text-slate-300 hover:bg-slate-700'
            }`}
          >
            {view.charAt(0).toUpperCase() + view.slice(1)}
          </button>
        ))}
      </div>

      {/* Overview */}
      {activeView === 'overview' && (
        <div className="space-y-6">
          <div className="bg-slate-800 p-6 rounded-lg border border-slate-700">
            <h2 className="text-2xl font-bold mb-4 text-purple-400">Core Equation</h2>
            <div className="bg-slate-900 p-4 rounded text-center font-mono text-xl mb-4">
              ∫(y(x) + ε)dx = ∫y(x)dx + εx + C
            </div>
            <p className="text-slate-300 leading-relaxed">
              The error term ε doesn't integrate to zero—it accumulates <span className="text-pink-400 font-semibold">linearly with time</span>. 
              This is the mathematical proof that unprocessed experience compounds as bias, tension, or pathology.
            </p>
          </div>

          <div className="grid md:grid-cols-3 gap-4">
            <div className="bg-gradient-to-br from-slate-800 to-slate-900 p-5 rounded-lg border border-purple-500/30">
              <div className="text-3xl mb-2">🏛️</div>
              <h3 className="font-bold text-lg mb-2 text-purple-300">The Problem</h3>
              <p className="text-sm text-slate-400">
                Compression without release creates pathological pressure. The dam will break.
              </p>
            </div>
            <div className="bg-gradient-to-br from-slate-800 to-slate-900 p-5 rounded-lg border border-pink-500/30">
              <div className="text-3xl mb-2">🎭</div>
              <h3 className="font-bold text-lg mb-2 text-pink-300">The Solution</h3>
              <p className="text-sm text-slate-400">
                Ritualized release transforms ε from debris into drive. Schedule the overflow.
              </p>
            </div>
            <div className="bg-gradient-to-br from-slate-800 to-slate-900 p-5 rounded-lg border border-blue-500/30">
              <div className="text-3xl mb-2">📖</div>
              <h3 className="font-bold text-lg mb-2 text-blue-300">The Result</h3>
              <p className="text-sm text-slate-400">
                Integration creates ΔS: the ledger of survived intensity becomes culture.
              </p>
            </div>
          </div>
        </div>
      )}

      {/* Reservoir View */}
      {activeView === 'reservoir' && (
        <div className="space-y-6">
          <div className="bg-slate-800 p-6 rounded-lg border border-slate-700">
            <h2 className="text-2xl font-bold mb-4 text-purple-400">ε Reservoir Dynamics</h2>
            <p className="text-slate-300 mb-6">
              With ritualized discharge every 7 days, the system maintains stable pressure. 
              The <span className="text-yellow-400">threshold</span> (8) and <span className="text-red-400">danger zone</span> (12) 
              show where compression becomes pathological.
            </p>
            <div className="bg-slate-900 p-4 rounded">
              <AreaChart width={800} height={400} data={reservoirData}>
                <defs>
                  <linearGradient id="colorEpsilon" x1="0" y1="0" x2="0" y2="1">
                    <stop offset="5%" stopColor="#a855f7" stopOpacity={0.8}/>
                    <stop offset="95%" stopColor="#a855f7" stopOpacity={0.1}/>
                  </linearGradient>
                </defs>
                <CartesianGrid strokeDasharray="3 3" stroke="#334155" />
                <XAxis dataKey="day" stroke="#94a3b8" label={{ value: 'Days', position: 'insideBottom', offset: -5, fill: '#94a3b8' }} />
                <YAxis stroke="#94a3b8" label={{ value: 'ε Accumulation', angle: -90, position: 'insideLeft', fill: '#94a3b8' }} />
                <Tooltip 
                  contentStyle={{ backgroundColor: '#1e293b', border: '1px solid #475569', borderRadius: '8px' }}
                  labelStyle={{ color: '#e2e8f0' }}
                />
                <ReferenceLine y={8} stroke="#facc15" strokeDasharray="3 3" label={{ value: 'Threshold', fill: '#facc15', position: 'right' }} />
                <ReferenceLine y={12} stroke="#ef4444" strokeDasharray="3 3" label={{ value: 'Danger', fill: '#ef4444', position: 'right' }} />
                <Area type="monotone" dataKey="epsilon" stroke="#a855f7" fill="url(#colorEpsilon)" strokeWidth={2} />
                <Line type="monotone" dataKey="ritual" stroke="#22c55e" strokeWidth={4} dot={{ fill: '#22c55e', r: 6 }} />
              </AreaChart>
            </div>
            <div className="mt-4 flex gap-4 items-center justify-center">
              <div className="flex items-center gap-2">
                <div className="w-4 h-4 bg-purple-500 rounded"></div>
                <span className="text-sm text-slate-300">ε Accumulation</span>
              </div>
              <div className="flex items-center gap-2">
                <div className="w-4 h-4 bg-green-500 rounded-full"></div>
                <span className="text-sm text-slate-300">Ritual Discharge</span>
              </div>
            </div>
          </div>
        </div>
      )}

      {/* Failure Mode */}
      {activeView === 'failure' && (
        <div className="space-y-6">
          <div className="bg-slate-800 p-6 rounded-lg border border-red-500/50">
            <h2 className="text-2xl font-bold mb-4 text-red-400">Pathological Accumulation</h2>
            <p className="text-slate-300 mb-6">
              Without scheduled release, ε accumulates past all thresholds. This is the mathematics of 
              breakdown: personal, social, civilizational. The <span className="text-red-400 font-semibold">crash is inevitable</span>, 
              only timing is uncertain.
            </p>
            <div className="bg-slate-900 p-4 rounded">
              <LineChart width={800} height={400} data={pathologicalData}>
                <CartesianGrid strokeDasharray="3 3" stroke="#334155" />
                <XAxis dataKey="day" stroke="#94a3b8" label={{ value: 'Days (No Rituals)', position: 'insideBottom', offset: -5, fill: '#94a3b8' }} />
                <YAxis stroke="#94a3b8" label={{ value: 'ε Accumulation', angle: -90, position: 'insideLeft', fill: '#94a3b8' }} />
                <Tooltip 
                  contentStyle={{ backgroundColor: '#1e293b', border: '1px solid #475569', borderRadius: '8px' }}
                  labelStyle={{ color: '#e2e8f0' }}
                />
                <ReferenceLine y={8} stroke="#facc15" strokeDasharray="3 3" label={{ value: 'Threshold', fill: '#facc15', position: 'right' }} />
                <ReferenceLine y={12} stroke="#ef4444" strokeDasharray="3 3" label={{ value: 'Danger', fill: '#ef4444', position: 'right' }} />
                <Line type="monotone" dataKey="epsilon" stroke="#ef4444" strokeWidth={3} dot={false} />
              </LineChart>
            </div>
          </div>

          <div className="grid md:grid-cols-3 gap-4">
            <div className="bg-slate-800 p-5 rounded-lg border border-slate-700">
              <h3 className="font-bold text-lg mb-2 text-slate-200">Apollonian Tyranny</h3>
              <p className="text-sm text-slate-400 mb-3">Infinite compression, no release</p>
              <p className="text-xs text-slate-500">French aristocracy 1789, Soviet apparatus 1991, individual psyche before breakdown</p>
            </div>
            <div className="bg-slate-800 p-5 rounded-lg border border-slate-700">
              <h3 className="font-bold text-lg mb-2 text-slate-200">Dionysian Flood</h3>
              <p className="text-sm text-slate-400 mb-3">Infinite variance, no container</p>
              <p className="text-xs text-slate-500">Addiction, mania, continuous catharsis without integration or learning</p>
            </div>
            <div className="bg-slate-800 p-5 rounded-lg border border-slate-700">
              <h3 className="font-bold text-lg mb-2 text-slate-200">Modern Arrhythmia</h3>
              <p className="text-sm text-slate-400 mb-3">Compression + suppression, pathologized release</p>
              <p className="text-xs text-slate-500">The worst synthesis: pressure builds with gauge painted over</p>
            </div>
          </div>
        </div>
      )}

      {/* Phases */}
      {activeView === 'phases' && (
        <div className="space-y-6">
          <div className="bg-slate-800 p-6 rounded-lg border border-slate-700">
            <h2 className="text-2xl font-bold mb-4 text-purple-400">The Five-Phase Cycle</h2>
            <p className="text-slate-300 mb-6">
              The Bacchic engine operates as a phase-locked loop, transforming chaos into culture through 
              rhythmic compression and release.
            </p>
          </div>

          <div className="space-y-4">
            {[
              { emoji: '🌱', phase: 'θ′ (Soil)', title: 'Variance', color: 'border-amber-700', desc: 'Raw ferment: wine, music, moonlight. The grape on the vine, buzzing with yeast and chance. Uncompressed noise.' },
              { emoji: '🍷', phase: 'θ (Roots)', title: 'Encoding', color: 'border-orange-600', desc: 'Fermentation: sugar becomes alcohol, chaos becomes energy. Priest encodes ritual. Costumes, drums, masks—interfaces that contain variance.' },
              { emoji: '🎵', phase: 'Σ (Trunk)', title: 'Compression', color: 'border-yellow-600', desc: 'Communal dance, chanting in unison. Individual ecstasy compresses into rhythm. Ritualization channels overflow into synchronization.' },
              { emoji: '🎭', phase: 'h(t) (Branch)', title: 'Explosion', color: 'border-red-600', desc: 'The god arrives, wine takes over, self dissolves. The differential explodes into curvature. Metamorphosis within, collision between. d²y/dx².' },
              { emoji: '📜', phase: 'ΔS (Canopy)', title: 'Integration', color: 'border-blue-600', desc: 'The hangover, the harvest, the storytelling. Society integrates what it learned in delirium. Laws, myths, tragedies arise. ∫y dx + εx + C.' }
            ].map((item, i) => (
              <div key={i} className={`bg-slate-800 p-5 rounded-lg border-l-4 ${item.color}`}>
                <div className="flex items-start gap-4">
                  <div className="text-4xl">{item.emoji}</div>
                  <div className="flex-1">
                    <h3 className="font-bold text-xl mb-1 text-slate-100">{item.phase}: {item.title}</h3>
                    <p className="text-slate-400 text-sm">{item.desc}</p>
                  </div>
                </div>
              </div>
            ))}
          </div>

          <div className="bg-gradient-to-r from-purple-900/50 to-pink-900/50 p-6 rounded-lg border border-purple-500/30">
            <h3 className="font-bold text-lg mb-3 text-purple-300">The Loop Closes</h3>
            <p className="text-slate-300 text-sm leading-relaxed">
              After integration, the cycle returns to variance (θ′) with <span className="text-pink-400 font-semibold">finer resolution</span>. 
              You're not building once—you're spiraling upward. Each rotation carves signal from residue, then feeds that residue back as input.
              The εx term becomes culture: character earned through tension.
            </p>
          </div>
        </div>
      )}

      {/* Application */}
      {activeView === 'application' && (
        <div className="space-y-6">
          <div className="bg-slate-800 p-6 rounded-lg border border-slate-700">
            <h2 className="text-2xl font-bold mb-4 text-purple-400">Operational Calendar Thermodynamics</h2>
            <p className="text-slate-300 mb-6">
              If you recognize ε building without outlet, the solution isn't spontaneity or harder work. 
              It's <span className="text-purple-400 font-semibold">engineered rhythm</span>.
            </p>
          </div>

          <div className="grid md:grid-cols-2 gap-6">
            <div className="space-y-4">
              <div className="bg-slate-800 p-5 rounded-lg border border-purple-500/30">
                <h3 className="font-bold text-lg mb-3 flex items-center gap-2">
                  <span className="text-2xl">📊</span>
                  <span className="text-purple-300">1. Measure the Reservoir</span>
                </h3>
                <p className="text-sm text-slate-400 mb-3">What's the unencoded variance?</p>
                <ul className="text-xs text-slate-500 space-y-1 list-disc list-inside">
                  <li>Jokes that didn't land</li>
                  <li>Ideas you censored</li>
                  <li>Anger you performed away</li>
                  <li>Desires redirected into productivity</li>
                </ul>
              </div>

              <div className="bg-slate-800 p-5 rounded-lg border border-pink-500/30">
                <h3 className="font-bold text-lg mb-3 flex items-center gap-2">
                  <span className="text-2xl">📅</span>
                  <span className="text-pink-300">2. Schedule the Ritual</span>
                </h3>
                <p className="text-sm text-slate-400 mb-3">Not "when it feels right"—regularly</p>
                <ul className="text-xs text-slate-500 space-y-1 list-disc list-inside">
                  <li>Weekly: Sabbath, creative time, movement</li>
                  <li>Monthly: Wilderness, deep work, solitude</li>
                  <li>Annual: Pilgrimage, transformation, risk</li>
                </ul>
                <p className="text-xs text-slate-400 mt-3 italic">
                  Frequency matters less than commitment to discharge
                </p>
              </div>
            </div>

            <div className="space-y-4">
              <div className="bg-slate-800 p-5 rounded-lg border border-blue-500/30">
                <h3 className="font-bold text-lg mb-3 flex items-center gap-2">
                  <span className="text-2xl">📝</span>
                  <span className="text-blue-300">3. Create Integration Space</span>
                </h3>
                <p className="text-sm text-slate-400 mb-3">After release comes sense-making</p>
                <ul className="text-xs text-slate-500 space-y-1 list-disc list-inside">
                  <li>Journal the overflow</li>
                  <li>Create from the residue</li>
                  <li>Talk through the transformation</li>
                  <li>Let εx become story, not static</li>
                </ul>
              </div>

              <div className="bg-slate-800 p-5 rounded-lg border border-green-500/30">
                <h3 className="font-bold text-lg mb-3 flex items-center gap-2">
                  <span className="text-2xl">🏛️</span>
                  <span className="text-green-300">4. Protect the Container</span>
                </h3>
                <p className="text-sm text-slate-400 mb-3">The ritual needs boundaries</p>
                <p className="text-xs text-slate-500">
                  Dionysus had his <em>temenos</em>, his sacred precinct. If every moment is available 
                  for overflow, none is. The bow is drawn and released in <span className="text-green-400 font-semibold">rhythm</span>—the 
                  heartbeat of becoming.
                </p>
              </div>
            </div>
          </div>

          <div className="bg-gradient-to-r from-slate-800 to-slate-900 p-6 rounded-lg border border-slate-700">
            <h3 className="font-bold text-xl mb-3 text-slate-200">Example Ritual Architectures</h3>
            <div className="grid md:grid-cols-3 gap-4">
              <div className="bg-slate-900/50 p-4 rounded">
                <h4 className="font-semibold text-purple-400 mb-2">Artist</h4>
                <p className="text-xs text-slate-400">Weekly: Studio chaos day. Monthly: Gallery visits. Annual: Residency/immersion</p>
              </div>
              <div className="bg-slate-900/50 p-4 rounded">
                <h4 className="font-semibold text-pink-400 mb-2">Executive</h4>
                <p className="text-xs text-slate-400">Weekly: Strategy void. Monthly: Off-grid retreat. Annual: Sabbatical/reinvention</p>
              </div>
              <div className="bg-slate-900/50 p-4 rounded">
                <h4 className="font-semibold text-blue-400 mb-2">Scholar</h4>
                <p className="text-xs text-slate-400">Weekly: Free writing. Monthly: Conference/salon. Annual: Fieldwork/adventure</p>
              </div>
            </div>
          </div>

          <div className="bg-gradient-to-br from-purple-900/30 to-pink-900/30 p-6 rounded-lg border border-purple-500/50">
            <h3 className="font-bold text-xl mb-3 text-purple-300">The Question</h3>
            <p className="text-slate-300 leading-relaxed">
              For any system—biological, social, artistic, personal—it's never "can we eliminate the noise?" 
              It's: <span className="text-pink-400 font-bold text-lg">"Have we built the festival that turns ε into signal 
              before it turns into catastrophe?"</span>
            </p>
          </div>
        </div>
      )}

      {/* Footer */}
      <div className="mt-12 pt-6 border-t border-slate-700 text-center text-slate-500 text-sm">
        <p>Dionysus wasn't the god of chaos.</p>
        <p className="text-purple-400">He was the god of <span className="font-semibold">scheduled chaos</span>.</p>
      </div>
    </div>
  );
};

export default BacchicEngine;
