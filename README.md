# Specify Design

Tato stránka prezentuje služby návrhu interiérů prostřednictvím přehledného a moderního rozhraní. Níže je textový popis struktury a funkcí webu.

---

## 🧭 Hlavička (Header)

- **Menu ikona**: Tlačítko s ikonou ☰ (`<i class="fas fa-bars"></i>`)
- **Název**: `SPECIFY` – ve středu horní části

---

## 🖼️ Obrázky (Image Row)

Dvě vedle sebe umístěné obrázky:
- `images/obrazek1.png` – *Obývací pokoj*
- `images/obrazek2.png` – *Kuchyně*

Oba obrázky mají:
- Rozměr 140×140 px
- Zaoblené rohy
- `object-fit: cover`

---

## 🛠️ Služby (Services)

Přehled nabízených služeb zobrazených v mřížce 2×2 + jedna služba přes celý řádek.

| Ikona                     | Popis služby                                 |
|--------------------------|----------------------------------------------|
| 🧭 `fa-drafting-compass` | 2D Náčrt prostoru a konzultace               |
| 🔁 `fa-sync-alt`         | 3D Model a export designu                    |
| ✏️ `fa-pencil-alt`       | 3D Design a VR prohlídka + konzultace       |
| 🥽 `fa-vr-cardboard`     | 3D Design a VR prohlídka + konzultace       |
| 👤 `fa-user`             | 3D Design a VR prohlídka + konzultace       |

Každá služba:
- Bílý box se zaoblením
- Při **hoveru**: mění barvu pozadí a textu

---

## 🖼️ Dekorace (Single Image)

Jeden velký obrázek ve spodní části:
- `images/obrazek3.png` – *Dekorace*

---

## 🎨 Styly (CSS)

Externí soubor `style.css` definuje:
- Flexbox pro rozvržení
- Barevné pozadí `#aef7ff`
- Styl pro obrázky, hover efekty, přechody (transition)
- Maximální šířka pro mobilní zobrazení (480px)
- Hover efekty pro: `.menu-icon`, `.title`, `.service-item`, `.service-item i`

```css
.menu-icon:hover,
.title:hover {
  color: #007bff;
}

.service-item:hover {
  background: #e0f8ff;
  color: #007bff;
}

.service-item:hover i {
  color: #007bff;
}
