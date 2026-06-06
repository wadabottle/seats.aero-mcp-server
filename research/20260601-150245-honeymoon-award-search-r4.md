# Honeymoon Award Flight Search — Round 4
**Run**: 2026-06-01 15:02 PT  
**Trigger**: Cross-referenced transfer-partners/ files against unsearched programs  
**New queries**: Turkish bulk (200), Qatar bulk (200), Singapore bulk (200), SFO→LHR expanded (50 results)  
**Builds on**: R3 (20260601-142006)

---

## New Programs Evaluated

### Turkish Miles&Smiles (Capital One → Turkish 1:1)

**SFO→IST outbound:**
| Date | Miles | Taxes | Seats | Airlines |
|------|-------|-------|-------|----------|
| Sep 21 | 135,000 | $0 | 5 ✓ | TK direct |
| Sep 22 | 135,000 | $0 | 5 ✓ | TK direct |
| Sep 24 | 135,000 | $0 | 3 | TK direct |
| Sep 20/23/25–29 | 135,000 | $0 | 0 ❌ | TK |

**IST→SFO return**: No results in bulk data.

**Verdict**: 135k Turkish miles for SFO→IST is overpriced for a gateway city. **Better use**: Turkish Miles&Smiles is renowned for cheap intra-Europe hops (IST→ATH, IST→FCO ~12–15k miles each). If the trip routes through Istanbul anyway, Capital One → Turkish could cover internal legs cheaply. Not useful for the longhaul.

---

### Qatar Privilege Club Avios (Amex/Capital One → Qatar 1:1, added Sep 2025)

**SFO-origin results (200-record bulk):**
| Date | Route | Miles | Taxes | Seats | Airlines |
|------|-------|-------|-------|-------|----------|
| Sep 28 | SFO→LHR | 180,000 | $0 | 1 ⚠️ | QR (via DOH) |
| Sep 28 | SFO→BCN | 180,000 | $0 | 1 ⚠️ | QR (via DOH) |
| Sep 28 | SFO→MAD | 180,000 | $0 | 1 ⚠️ | QR (via DOH) |

**Verdict**: Taxes are zero (Qatar doesn't impose fuel surcharges on Avios bookings) but 180k miles is well into overpriced tier and only 1 seat. Not viable for a couple at current availability.

---

### Singapore KrisFlyer (Amex/Capital One/Chase → SQ 1:1)

**Result**: All seats.aero SQ data is JFK→FRA fifth-freedom routes (Singapore Airlines operates NYC→Frankfurt). No SFO-origin routes exist. **Dead end from SFO** — would require positioning to JFK.

---

### American AAdvantage via SFO→LHR (expanded 50-result search)

This is the sleeper finding. AAdvantage shows SFO→LHR at **57,500 miles** — sweet-spot pricing — but every date shows **0 seats**:

| Date | Miles | Taxes | Seats | Operated by |
|------|-------|-------|-------|-------------|
| Sep 20 | 57,500 | $164 | 0 ❌ | IB (Iberia) |
| Sep 27 | 57,500 | $733 | 0 ❌ | BA (direct) |
| Sep 28 | 57,500 | $748 | 0 ❌ | AA/BA |
| Oct 5 | 57,500 | $733 | 0 ❌ | AA/AS/BA (direct) |

57,500 AAdvantage miles for SFO→LHR in business is legitimately sweet-spot pricing. AA transfers from Chase (1:1), and Iberia Plus Avios (Amex 1:1) can also book AA metal at similar rates. **Monitor weekly** — if BA or AA releases seats, this becomes the best outbound option by a wide margin.

---

## No Change to Current Best Booking

The transfer files don't unlock anything immediately bookable better than the current Flying Blue options. The standings are unchanged:

### Best Available Round Trip
**SFO→LHR Sep 28 (FB, 115.5k + $367) + AMS→SFO Oct 7 (FB, 129k + $423)**  
489,000 Flying Blue total | ~$1,580 taxes for 2

### Points Plan
| Transfer | Amount | To | Purpose |
|----------|--------|----|---------|
| Amex → Flying Blue | 270,000 | FB | Covers most of both legs |
| Capital One → Flying Blue | ~219,000 | FB | Tops off remainder |
| Chase (keep) | 38,500 | — | Reserve for AA if seats open |

---

## Updated Monitoring Priority

| Priority | Signal | Program | Action |
|----------|--------|---------|--------|
| 🔥 1 | AA/BA SFO→LHR at 57,500 seats appear | AAdvantage (Chase) or Iberia/BA Avios (Amex/Chase) | Book immediately; best rate found |
| 🔥 2 | Aeroplan SFO→ZRH/FRA partner release | Aeroplan (Amex/C1/Chase) | ~75–90k miles + ~$50 fees; beats everything |
| 3 | Virgin Atlantic SFO→LHR dips below 100k | Virgin Atlantic (Amex) | Switch outbound from FB; nonstop premium |
| 4 | Amex→VA 40% transfer bonus | Virgin Atlantic | Effective ~100k Amex for nonstop outbound |
| 5 | FB Promo Rewards includes US-Europe biz | Flying Blue | Sub-60k miles possible; check monthly |

---

## Searches Run (Round 4)

| Query | File / Result | Key finding |
|-------|--------------|------------|
| Turkish bulk 200 NA→Europe Sep20–Oct5 | mcp-seats-get_bulk_avail-1780351292518.txt | SFO→IST at 135k/$0, 5 seats Sep 21/22 |
| Singapore bulk 200 NA→Europe | (inline — 12 records) | JFK→FRA only via SQ; no SFO |
| Qatar bulk 200 NA→Europe Sep20–Oct5 | mcp-seats-get_bulk_avail-1780351294841.txt | SFO→LHR/BCN/MAD at 180k/$0, 1 seat only |
| SFO→LHR all programs, 50 results | mcp-seats-get_flights-1780351296192.txt | AA at 57.5k/$0–$748, 0 seats; confirms FB/VA rankings |
