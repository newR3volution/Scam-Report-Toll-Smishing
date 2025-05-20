# Case: Toll of Deception – Fake DMV SMS Threat

**Date Reported:** May 2025  
**Scam Type:** SMS Phishing (Spoofed Government Notice)  
**Scam Score:** HIGH  
**Framework:** Scam Tactic Chain v2  
**Status:** Documented – Public Awareness  

## Summary
A phishing SMS impersonates the **Florida Highway Safety and Motor Vehicles (FLHSMV)** to threaten legal action over an alleged toll violation. The message pressures the recipient to pay immediately or face vehicle suspension, legal penalties, and credit damage. The message is built entirely on manufactured fear, a spoofed URL, and misused legal language.
Despite its aggressive tone, the scam collapses under scrutiny:
- The recipient **has not lived in Florida in years**
- The sender is a **Philippine number**
- The URL ends in **`.win`**, not `.gov`
- The grammar is broken (“May 22st”)

This is a textbook example of a **disruption-based phishing attack** built to shock and extract compliance.

*While the scam message in this case spoofed Florida's DMV system, the victim no longer resides in Florida. However, this incident aligns with a broader trend of regionally tailored smishing campaigns. Interestingly, the recipient's spouse, still based in Oklahoma, has only received Oklahoma-specific phishing messages, while the Florida-themed message targeted someone with previous ties to that state. This indicates the attacker may be working with partial or outdated location data from breaches, public records, or data brokers to personalize these messages just enough to bypass skepticism.*

## STC v2 Breakdown

### 1. **Disruption**
The attacker seizes the target’s attention with an alarming and unexpected message:
- “Final Notice” framing triggers **fight-or-flight**
- Legal phrases (“illegal driver,” “credit damage,” “enforcement”) disorient and overwhelm
- The threat of government action **bypasses rational skepticism**

### 2. **Control**
The attacker then narrows the victim’s options:
- Link to `flhsmv.gov-flb.win/us` mimics a trusted domain  
- Uses state authority (FLHSMV) to create legitimacy  
- Message says “Reply Y” — conditioning the victim to obey without thinking  
- Creates the illusion that **failure to act equals legal punishment**

### 3. **Compliance**
The victim is funneled toward action:
- Click the link (likely a phishing/payment page)  
- Or reply directly, risking additional social engineering  
- The scam offers **no verification path**, only one outcome: **pay or suffer**

### 4. **Aftermath**
If successful, the attacker may:
- Steal credit card or personal data  
- Install malware through the link  
- Harvest reply data for further scams  
- Cause emotional distress and financial harm  

## Red Flags

- **Out-of-State Claim**: Recipient has no ties to Florida  
- **International Origin**: `+63` Philippines number used  
- **Spoofed Domain**: `.win` TLD impersonating `.gov`  
- **Grammar Error**: “May 22st”  
- **Unsolicited Threat**: Real toll authorities do not use SMS this way  


## Scam Message (Redacted)

**From:** `+63 912 XXX XXXX`  
**Content:**
“Final Notice: Enforcement will begin after May 22st.
You will face legal action for driving as an illegal driver,
and this will damage your credit. Please pay before enforcement:
https://flhsmv.gov-flb.win/us

Reply Y and re-open this message.”

## Detection Tips

- Legitimate agencies use **mail, not international SMS**  
- Government sites in the U.S. end in **.gov**, not `.win`  
- Misspellings and urgent threats are **hallmarks of scam attempts**  
- Never respond or click unsolicited links from unknown numbers  
- Search for the official site directly if in doubt  
