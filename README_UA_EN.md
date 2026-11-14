# Mars Explorer AI · Martian Map v008 — release audit

## Українська
v008 — аудит локального пакета v007 перед публікацією. Збережено діючі режими NASA Mars Trek MOLA/HiRISE, схему Єзеро, демонстрацію Dijkstra/A*, результати Kaggle v026 та імпорт GeoJSON. Виправлено версію у верхньому заголовку в обох мовах. Додано панель аудиту й `RELEASE_AUDIT_v008.json`.

Перевірено локальний маніфест v007 (7 із 7 файлів); порівняно файли CSV v026 із наявними локальними результатами; перераховано підсумки з 14 рядків, 7 вікон і двох запасів похилу; перевірено каталог 70 Notebook та структуру маніфесту із 76 записами. **Локальна перевірка SHA-256 НЕ є зовнішньою автентифікацією чи незалежною науковою реплікацією.**

Геологічні полігони USGS НЕ вбудовані, просторова реєстрація не перевірена, A*/Dijkstra з v026 НЕ є фізичними маршрутами по карті Єзеро. Оригінальні архіви фаз III–V мають невирішені розбіжності зовнішніх SHA. Дизайн для конкурсної демонстрації — дослідницький прототип, не сертифікована навігація.

## English
v008 audits the local v007 release package ahead of publication. It retains NASA MOLA/HiRISE tiles, the Jezero overview, Dijkstra/A* synthetic demonstration, Kaggle v026 results, and GeoJSON geology importer. Both language versions now show v008 in the top heading. A QA banner links to `RELEASE_AUDIT_v008.json`.

Local checks include the v007 manifest (7/7 files), byte-level comparison against locally available v026 experiment outputs, recomputation of summaries from 14 rows covering 7 windows and two slope margins, the 70-notebook catalog, and 76 export manifest records. **Local SHA-256 checks are not external authentication or independent scientific replication.**

USGS polygons are not bundled; map coordinate registration remains unverified; v026 algorithmic paths are NOT physical routes in Jezero. Original phase-release ZIP SHA mismatches for III–V remain unresolved. Research prototype only — no certified navigation or physical safety claims.

## Usage
Unzip, open `index.html` in Chrome/Edge. For local CSV SHA checking via Fetch/WebCrypto, run `python -m http.server 8000` in the extracted folder and open `http://localhost:8000/` (local `file://` may block fetch). NASA Mars Trek tile loads require internet.

## Public evidence
- https://www.kaggle.com/datasets/olekis/mars-explorer-ai-research-code-v001-v070
- https://www.kaggle.com/code/olekis/mars-explorer-ai-70-experiments-research-code
- https://trek.nasa.gov/mars/
- https://pubs.usgs.gov/sim/3464/
