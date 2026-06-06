# Honeymoon Award Flight Search — Round 3
**Run**: 2026-06-01 14:20 PT  
**New queries**: Aeroplan + United outbound (ZRH/FRA/MUC); same routes return; United bulk 1,000 results  
**Builds on**: R2 (20260601-115040), benchmarks (20260601-140435)

---

## Key Finding: The Lufthansa Trap

All SFO→ZRH/FRA/MUC results return exclusively under the **Lufthansa Miles & More** program — not Aeroplan, not United. The seats are abundant (5–6 per flight on many dates) but the fees are brutal.

| Route | Dates with 2+ seats | Miles | Taxes | Program |
|-------|--------------------|----|------|---------|
| SFO → ZRH | Sep 22, 23, 28, 29, Oct 4, 5 | 75,420–87,415 | $1,046–$1,246 | Lufthansa (M&M) |
| SFO → FRA | Sep 22, 23, 24, 28, 29, Oct 5 | 75,420–88,381 | $1,046–$1,207 | Lufthansa (M&M) |
| SFO → MUC | Sep 21, 22, 23, 24, 28, 29, 30, Oct 2, 5 | 74,811–87,415 | $1,046–$1,207 | Lufthansa (M&M) |

**The problem**: Lufthansa's own program passes on $1,000–$1,400 carrier-imposed surcharges. Same flights booked via **Aeroplan** would carry ~$50 in taxes — but Aeroplan doesn't currently have partner release on SFO→Europe routes (confirmed: zero Aeroplan SFO results in 1,000-record bulk pull).

**The opportunity**: If Aeroplan releases SFO partner inventory, these same seats at 75–90k miles + ~$50 fees would be the best transatlantic business class redemption available. Worth monitoring weekly on seats.aero.

---

## United: Confirmed Dead End

Pulled 1,000 results from United bulk (NA→Europe business, Sep 20–Oct 5). **Zero SFO-origin routes.** United has no SFO→Europe business class award availability in this window at any price.

> Note: Amex→United transfers are valid but irrelevant here — there are no seats to book.

---

## Return: ZRH/FRA/MUC → SFO

| Route | Results |
|-------|---------|
| ZRH → SFO | ❌ Zero results |
| FRA → SFO | ❌ Zero results |
| MUC → SFO | Oct 7 only — Lufthansa, 81,392 miles, $842 taxes, 3 seats, not direct |

MUC→SFO via Lufthansa: fees still too high at $842/person. Same problem as outbound.

---

## Consolidated Best Options (All Rounds)

### Outbound SFO → Europe (Business, 2+ seats)

| Rank | Date | Route | Program | Miles/pax | Fees/pax | Seats | Notes |
|------|------|-------|---------|-----------|---------|-------|-------|
| ⭐ 1 | Sep 28 | SFO → LHR | Flying Blue | 115,500 | $367 | 9 | Best value; AF (1 stop) |
| 2 | Sep 27 | SFO → LHR | Virgin Atlantic | 140,000 | $699 | 9 | Only nonstop VS direct |
| 3 | Oct 3 | SFO → LHR | Virgin Atlantic | 130,000 | $699 | 9 | Nonstop, better miles |
| 4 | Sep 28 | SFO → ATH | Flying Blue | 176,000 | $366 | 4 | Greece-first routing |
| 5 | Sep 22–Oct 5 | SFO → ZRH/FRA/MUC | Lufthansa M&M | 74,811–88,381 | $1,046–$1,246 | 4–6 | ⛔ Fees kill the value |

### Return Europe → SFO (Business, 2+ seats)

| Rank | Date | Route | Program | Miles/pax | Fees/pax | Seats | Notes |
|------|------|-------|---------|-----------|---------|-------|-------|
| ⭐ 1 | Oct 7 | AMS → SFO | Flying Blue | 129,000 | $423 | 3 | Direct KLM |
| 2 | Oct 7/9 | CDG → SFO | Flying Blue | 129,000 | $511 | 8 | Great inventory |
| 3 | Oct 9 | AMS → SFO | Flying Blue | 129,000 | $423 | 2 | KL/VS |

---

## Best Round-Trip Itinerary: Current Best Available

**SFO → LHR (Sep 28, FB 115.5k + $367) → Italy → Greece → AMS → SFO (Oct 7, FB 129k + $423)**

| | Per person | 2 pax total |
|---|---|---|
| Miles | 244,500 FB | **489,000 FB** |
| Taxes | $790 | **~$1,580** |
| Points needed | Amex 270k + C1 200k → FB = 470k; Chase 38.5k tops off gap | |

---

## Monitoring Priority

| Signal | Action |
|--------|--------|
| Aeroplan SFO→ZRH/FRA/MUC appears in seats.aero | Book immediately at ~75–90k miles + ~$50 fees — best possible redemption |
| Virgin Atlantic SFO→LHR drops below 100k miles | Consider switching outbound from FB to VA for the nonstop |
| Flying Blue Promo Rewards includes US-Europe business | Sub-60k miles possible; check monthly |
| Amex → Virgin Atlantic transfer bonus announced | 40% bonus effectively cuts 140k VA rate to ~100k Amex — reconsider VA outbound |

---

## Searches Run (Round 3)

| Query | File | Key finding |
|-------|------|------------|
| SFO→ZRH business Sep20–Oct5 | mcp-seats-get_flights-1780348698371.txt | LH only, $1,046–$1,246 fees |
| SFO→FRA business Sep20–Oct5 | mcp-seats-get_flights-1780348700004.txt | LH only, $1,046–$1,207 fees |
| SFO→MUC business Sep20–Oct5 | mcp-seats-get_flights-1780348701526.txt | LH only, $1,046–$1,246 fees |
| ZRH→SFO business Oct5–Oct14 | mcp-seats-get_flights-1780348702830.txt | 0 results |
| FRA→SFO business Oct5–Oct14 | mcp-seats-get_flights-1780348704426.txt | 0 results |
| MUC→SFO business Oct5–Oct14 | mcp-seats-get_flights-1780348705609.txt | 1 result, LH, $842 fees |
| United bulk 1,000 NA→Europe | mcp-seats-get_bulk_avail-1780348724037.txt | 0 SFO-origin results |
