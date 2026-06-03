# EthosAI CLIM — Claiming & PR Evidence (PUBLIC)

> **Sichtbarkeit: ÖFFENTLICH. Nur redigierte, freigegebene Claiming-Evidenz.**
> **Visibility: PUBLIC. Redacted, released claiming evidence only.**

Dieses Repository enthält **öffentlich freigegebene** Belege für
Werbung/Öffentlichkeitsarbeit und überprüfbare Produkt-Claims von
EthosAI CLIM — z. B. dass eine autonome Brücken-Engineering-Pipeline real ein
GLB-Modell, BOM, Renders und eine LLM-Selbstabnahme erzeugt.

This repository holds **publicly released**, redacted evidence for marketing/PR
and verifiable product claims of EthosAI CLIM.

## Zweck / Purpose

- Pro Claim ein redigiertes Bundle: kundenneutrale Renders + GLB +
  **signiertes MANIFEST**.
- Das MANIFEST referenziert per **SHA-256-Hash das private Original** im
  internen Audit-Repo `ethos_ai_clim_evidence` → geschlossene, prüfbare
  Beweiskette ohne Offenlegung von IP oder Mandantendaten.

## Harte Regeln / Hard rules

1. **Nur Freigegebenes.** Inhalte erscheinen hier nur nach bewusster, redigierter
   Freigabe.
2. **Keine Kunden-/Mandantendaten.** Keine Kundennamen, keine vertraulichen
   Maße/Designs (EthosAI Sanitize-Regel).
3. **Keine Kern-IP.** Prompts, System-Prompts und Selbstabnahme-Logik bleiben im
   privaten Repo bzw. im Produkt.
4. **Hash-verankert.** Jeder öffentliche Claim trägt den Hash seines privaten
   Originals; Manipulation wird durch den Vergleich beider Seiten erkennbar.

## Bundle-Struktur / Bundle layout

```
<claim-id>/
  renders/           # kundenneutrale Kamera-Renders (PNG)
  model.glb          # redigiertes 3D-Ergebnis
  MANIFEST.json      # öffentliche Provenance + SHA-256 (inkl. Hash des privaten Originals)
  MANIFEST.sig       # Signatur über MANIFEST.json
```

## Ehrlichkeitsgrenze / Honesty boundary

Jedes Bundle kennzeichnet offen, welche Schritte **automatisiert** und welche
**interaktiv** erzeugt wurden. Es werden keine vollautomatischen Fähigkeiten
behauptet, die noch interaktive Schritte erfordern.
