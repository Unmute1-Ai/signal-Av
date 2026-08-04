# signal-Av
ASL intent bridge for autonomous vehicles — translating signed communication into safe, auditable context for Alpamayo-class driving AI.
signal-Av/
├── README.md
├── LICENSE
├── pyproject.toml
│
├── signal_av/
│   ├── perception/
│   │   ├── hand_tracking.py
│   │   ├── pose_tracking.py
│   │   └── facial_features.py
│   │
│   ├── asl/
│   │   ├── temporal_encoder.py
│   │   ├── intent_decoder.py
│   │   └── vocabulary.py
│   │
│   ├── intent/
│   │   ├── schema.py
│   │   ├── confidence.py
│   │   └── spatial_context.py
│   │
│   ├── safety/
│   │   ├── policy_gate.py
│   │   ├── phaseflow.py
│   │   └── audit.py
│   │
│   └── adapters/
│       ├── alpamayo.py
│       └── alpasim_grpc.py
│
├── proto/
│   └── signal_av.proto
│
├── tests/
│   ├── test_intent.py
│   ├── test_safety_gate.py
│   └── test_alpamayo_adapter.py
│
└── examples/
    └── pedestrian_stop_sign.py