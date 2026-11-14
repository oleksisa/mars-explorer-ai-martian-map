# Mars Explorer AI — v008 QA / checklist

## UA — перед поданням
- [x] Звірено 7/7 записів маніфесту попередньої локальної збірки v007.
- [x] Вбудовані CSV v026 збігаються байт у байт із доступними локальними результатами v026.
- [x] Перераховано підсумки для 14 рядків, 7 вікон і двох значень запасу похилу (0°, 5°).
- [x] Каталог містить 70 Notebook, експортний маніфест — 76 записів.
- [x] Chromium DOM/inline JavaScript: UA/EN, 4 вкладки, перемикання запасу похилу, 34.00/51.60, 132 вузли, 0 JS-помилок.
- [ ] Відкрити розпакований HTML у своєму Chrome та перевірити MOLA/HiRISE у v008 (працювали на скриншотах v004–v007).
- [ ] Перевірити SHA-кнопку через локальний HTTP сервер або публічний HTTPS (у `file://` fetch може блокуватися).
- [ ] Перевірити мобільне відображення та всі зовнішні посилання.
- [ ] Оприлюднити сайт для суддів та перевірити доступність без входу.
- [ ] Підтвердити відповідність умовам конкретного виклику, включно з попередньою роботою.

### Наукові застереження
USGS полігони не включено. Немає незалежно підтвердженої просторової реєстрації та геодезичних контрольних точок; маршрути v026 не накладені на реальну карту Єзеро; фізична безпека не перевірена. SHA маніфест локальний, не є зовнішнім засвідченням оригінальних даних NASA. Відомі розбіжності оригінальних ZIP SHA фаз III–V зберігаються.

## EN — prior to submission
- [x] Previous v007 local manifest 7/7 files match.
- [x] Bundled v026 CSV bytes match locally available experiment outputs.
- [x] Independently recomputed summary rows: 14 comparisons, 7 windows, 0°/5° margins.
- [x] Catalog: 70 notebooks; exported manifest: 76 records.
- [x] Chromium DOM/inline JS: language switches, all tabs, margin switch, 34.00/51.60, 132 nodes, no uncaught errors.
- [ ] Manually test MOLA/HiRISE tile loading in v008 Chrome; earlier v004–v007 screenshots confirm those versions.
- [ ] Test local CSV audit button over HTTP(S), not file://.
- [ ] Test mobile layout and every external link.
- [ ] Publish to a public URL accessible without authentication.
- [ ] Confirm competition rules for pre-existing research and the selected challenge.

### Scientific limitations
USGS geology polygons not bundled; no independent geographic registration or geodetic controls; v026 paths are not spatially mapped to Jezero; no physical route safety validation. Local SHA checks do not externally authenticate NASA products. Prior original phase-release ZIP SHA mismatches for III–V remain unresolved.
