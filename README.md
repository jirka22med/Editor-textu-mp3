🖖 Máš pravdu, více admirále Jiříku! Porušil jsem rozkaz - měl jsem používat TVÉ IRL Brackets číslování! 🚀

⚠️ OPRAVA MANUÁLU - S TVÝMI BRACKETS ČÍSLY
Pusť mi najít všechny tvé IRL Brackets komentáře v celém souboru, abych ti dal přesné instrukce s čísly řádků!Viewed 3 files, ran a commandHledám VŠECHNY Brackets komentáře pro přesné řádkováníScriptZobrazuji sekci kolem řádku 939-952 (Brackets komentář)Zobrazuji sekci kolem řádku 1042-1049 (Brackets komentář)Zobrazuji sekci kolem řádku 1189-1203 (Brackets komentář)Done🖖 PERFEKTNÍ! Teď mám VŠECHNY tvé IRL Brackets komentáře! 🚀

📋 OPRAVENÝ MANUÁL S TVÝMI IRL BRACKETS ČÍSLY

ČÁST 1: HTML - Nové Mobile Slidery
📍 Vlož po řádku 211 (tam kde končí tvůj první Brackets blok)
html<!-- 📱 MOBILE FONT SIZE SLIDERY - Více admirál Jiřík -->
<div class="setting-item">
    <label for="mobile-header-font-size">📱 Mobil - Velikost nadpisu (Header):</label>
    <div style="display:flex; align-items:center; gap:10px;">
        <input type="range" id="mobile-header-font-size" class="range-input" min="12" max="28" value="18">
        <span class="range-value" id="mobile-header-value">18px</span>
    </div>
</div>

<div class="setting-item">
    <label for="mobile-track-title-font-size">📱 Mobil - Velikost názvu skladby:</label>
    <div style="display:flex; align-items:center; gap:10px;">
        <input type="range" id="mobile-track-title-font-size" class="range-input" min="10" max="24" value="16">
        <span class="range-value" id="mobile-track-value">16px</span>
    </div>
</div>

ČÁST 2: currentSettings
📍 Řádek 33-34 (hned za headerFontSizePx a trackTitleFontSizePx)
javascriptheaderFontSizePx: 24,
trackTitleFontSizePx: 20,
mobileHeaderFontSizePx: 18,        // 📱 NOVÉ
mobileTrackTitleFontSizePx: 16,    // 📱 NOVÉ

ČÁST 3: loadSettingsToForm()
📍 Řádek 952 (hned za tvůj Brackets konec //<!-- řádek 952 brackets řádkování konec -->)
javascript//<!-- řádek 952 brackets řádkování konec      -->

// 📱 NOVÉ - Mobile font sizes
const mobileHeaderFontInput = this.DOM.modal.querySelector('#mobile-header-font-size');
if (mobileHeaderFontInput && this.currentSettings.mobileHeaderFontSizePx) {
    mobileHeaderFontInput.value = this.currentSettings.mobileHeaderFontSizePx;
    this.updateRangeValue(mobileHeaderFontInput);
}

const mobileTrackTitleFontInput = this.DOM.modal.querySelector('#mobile-track-title-font-size');
if (mobileTrackTitleFontInput && this.currentSettings.mobileTrackTitleFontSizePx) {
    mobileTrackTitleFontInput.value = this.currentSettings.mobileTrackTitleFontSizePx;
    this.updateRangeValue(mobileTrackTitleFontInput);
}

ČÁST 4: getSettingsFromForm()
📍 Řádek 1049 (hned za tvůj Brackets konec //<!-- řádek 1049 brackets řádkování konec -->)
javascript//<!-- řádek 1049 brackets řádkování konec      -->

// 📱 NOVÉ - Mobile font sizes
const mobileHeaderFontInput = this.DOM.modal.querySelector('#mobile-header-font-size');
if (mobileHeaderFontInput) newSettings.mobileHeaderFontSizePx = parseInt(mobileHeaderFontInput.value);

const mobileTrackTitleFontInput = this.DOM.modal.querySelector('#mobile-track-title-font-size');
if (mobileTrackTitleFontInput) newSettings.mobileTrackTitleFontSizePx = parseInt(mobileTrackTitleFontInput.value);

ČÁST 5: applySettings() - CSS
📍 Řádek 1203 (hned za tvůj Brackets konec //<!-- řádek 1203 brackets řádkování konec -->)
javascript//<!-- řádek 1203 brackets řádkování konec      -->

// 📱 NOVÉ - Mobile responsive font sizes
const mobileH1Size = settings.mobileHeaderFontSizePx || 18;
const mobileH2Size = settings.mobileTrackTitleFontSizePx || 16;

customCSS += `
    @media (max-width: 768px) {
        h1#nazev-prehravace {
            font-size: ${mobileH1Size}px !important;
        }
        h2#trackTitle {
            font-size: ${mobileH2Size}px !important;
        }
    }
`;

✅ KONTROLNÍ SEZNAM S IRL BRACKETS ČÍSLY:

 Řádek 211+ - HTML slidery vloženy
 Řádek 33-34 - currentSettings rozšířeny
 Řádek 952+ - loadSettingsToForm() doplněno
 Řádek 1049+ - getSettingsFromForm() doplněno
 Řádek 1203+ - applySettings() CSS media query přidáno


Teď máš manuál s TVÝMI IRL BRACKETS čísly, veliteli! 💾🔥🖖
