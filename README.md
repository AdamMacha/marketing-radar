# MarketingRadar 🚀

Autonomní systém pro akvizici B2B klientů pro marketingové agentury.

## Funkce systému
1. **Hledání firem (Google Places API)** – vyhledávání podle oborů (e-shopy, kliniky, developerské projekty, gastro, řemesla) a lokalit s automatickou dedupikací.
2. **Marketingový analyzér**:
   - Detekce a přítomnost profilů na sociálních sítích (Facebook, Instagram, LinkedIn, TikTok).
   - Analýza Google hodnocení a recenzí (reputace firmy).
   - Mobilní rychlost a PageSpeed výkon (klíčové pro placené kampaně).
   - Detekce měřicích kódů (Meta Pixel, Google Tag Manager, Google Analytics, Sklik).
3. **AI generování auditů & outreach (Google Gemini)**:
   - Veřejná microsite rozboru na `/a/[slug]` s doporučeními v oblasti marketingu, reklam a webu.
   - Osobní cold outreach e-mail, scénář pro telefonát a LinkedIn zpráva.
4. **Autopilot kampaně (Cron)**:
   - Rotace nik a lokalit, automatické prohledávání a příprava náhledů nebo přímé odesílání přes SMTP.
5. **Mini CRM**:
   - Stavy pipeline (nový, osloven, reagoval, schůzka, nabídka, vyhráno, prohráno), poznámky a historie aktivit.

## Rychlý start
```bash
npm install
cp .env.example .env.local
# Doplň proměnné v .env.local a spusť supabase/schema.sql ve své Supabase databázi
npm run dev
```
