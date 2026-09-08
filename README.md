- Estilização: TailwindCSS, darkmode.
- Linguagens: PHP, JS, HTML.
- Banco de dados: MySQL, dados de acesso ficam no arquivo .env (DB_HOST, DB_NAME, DB_USER, DB_PASS).
- Padrão arquitetural: Front Controller, combinado com Routing/Dispatcher.
- Endereço dos arquivo do app: public_html/subdrill/
- public_html/subdrill/app.index é o arquivo do Front Controller.

- Geração de respostas em texto:
API Key do Gemini, fica no arquivo .env (GEMINI_API_KEY).
define('GEMINI_API_KEY', envValue('GEMINI_API_KEY', ''));
define('GEMINI_API_URL', envValue('GEMINI_API_URL', 'https://generativelanguage.googleapis.com/v1beta/models'));
define('GEMINI_TRANSLATION_MODEL', envValue('GEMINI_TRANSLATION_MODEL', 'gemini-3.5-flash-lite'));

- Geração de áudios TTS:
API Key do Google Cloud, fica no arquivo .env (GOOGLE_CLOUD_API_KEY).
define('GOOGLE_CLOUD_API_KEY', envValue('GOOGLE_CLOUD_API_KEY', ''));
- ID das vozes:
Português: 'pt-BR-Chirp3-HD-Algenib'
Inglês: 'en-GB-Chirp3-HD-Achird'
