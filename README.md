# ProMaestro Voice v3.0 — Cognitive-Auditory Investment Framework  
*An experimental case of real-time voice-driven financial reasoning with ChatGPT.*

---

## 1. Overview  
`ProMaestro Voice v3.0` demonstrates how a single user can transform ChatGPT into a **cognitive-auditory copilot** for equity research and portfolio analysis.  
The framework merges spoken interaction, quantitative modeling (JSON schemas), and decision logic into one continuous reasoning loop:

> **Thought → Voice → AI Processing → Voice Feedback → Human Analysis → Voice Response**

This loop removes friction between thinking and execution, enabling high-speed analysis without keyboards or screens.

---

## 2. Core Concept  
Each company under coverage lives in its own conversational thread that stores financial reports, 10-Q/10-K filings, and presentation data.  
The AI extracts metrics, populates a standardized JSON structure, and delivers an auditory verdict under **two possible scenarios**:

| Scenario | Criteria | Action |
|-----------|-----------|--------|
| **Compounder** | ≥ 5× expected multiplier, sustained growth, controlled risk | Maintain / moderate increase |
| **TenBagger** | ≥ 10× potential, accelerated growth, high asymmetry | Strategic increase |

If neither condition is met → *No Go.*

---

## 3. Technical Architecture  

**Modules**  
1. **Data Ingestion** — Financial documents parsed directly inside ChatGPT.  
2. **ProMaestro JSON Schema** — Defines metrics, scenarios, risk flags, and 5-year projections.  
3. **Analytical Engine** — Calculates *expected multiplier*, *prob ≥ 10×*, *Rule of 40*, dilution, etc.  
4. **Voice Output v2.0** — Condenses the result into a 20-second spoken summary (dual-scenario).  
5. **Flag System** — Green / Red signals with Kill-Switch triggers.  
6. **Quarterly Loop** — Each thread updates every fiscal quarter; outputs feed an annual consolidated table.

---

## 4. Example Command





{
  "version": "v3.0",
  "framework": "ProMaestro Voice – Cognitive Auditory Investment Model",
  "as_of": "2025-10-05",
  "core_metrics": {
    "rev_cagr_3y": "Revenue CAGR (3 years)",
    "gm": "Gross Margin",
    "opm": "Operating Margin",
    "fcf_margin": "Free Cash Flow Margin",
    "rule_of_40": "Growth + Profitability Rule",
    "recurring_revenue_pct": "Recurring Revenue %",
    "nrr": "Net Revenue Retention",
    "rd_to_sales": "R&D to Sales",
    "sbc_to_sales": "Stock-Based Comp. to Sales",
    "dilution_3y": "Share Dilution (3 years)",
    "net_debt_to_ebitda": "Leverage Ratio",
    "ev_to_sales": "Enterprise Value / Sales",
    "ev_to_ebit": "Enterprise Value / EBIT"
  },
  "qualitative_factors": {
    "moat_types": ["switching_costs", "data_networks", "brand", "ecosystem"],
    "evidence_required": "Narrative proof from earnings calls or filings"
  },
  "tam_analysis": {
    "now": "Current TAM in USD",
    "cagr": "Expected TAM CAGR",
    "expansion_paths": ["Sector adjacencies", "AI extensions", "Geographic scaling"]
  },
  "output_metrics": {
    "prob_ge_10x": "Probability of >=10x over 5 years",
    "expected_multiplier": "Expected Portfolio Multiplier (5Y)",
    "compounder_score": "0–100 index for sustained compounding",
    "tenbagger_score": "0–100 index for high asymmetry growth"
  },
  "verdict_classes": {
    "1": "Compounder ≥ 5x (risk-controlled, NRR>1.15, GM>70%)",
    "2": "TenBagger ≥ 10x (high-growth asymmetry, TRV>35%)",
    "3": "Neutral/Undetermined"
  }
}
