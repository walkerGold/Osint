# Osint

---

Guia de Google Dorks para OSINT e Segurança

Aviso ⚠️

O uso de dorks deve ser feito de forma ética e legal. Invadir sistemas, acessar dados protegidos ou violar a privacidade de terceiros pode ser crime. Utilize este guia apenas para fins educativos e para testar a segurança de seus próprios sistemas.


---

# 📌 O que são Dorks?

Dorks são consultas avançadas usadas em mecanismos de busca, como o Google, para encontrar informações específicas que não aparecem facilmente nos resultados comuns. São amplamente utilizados em OSINT (Open Source Intelligence) e na segurança da informação para auditorias e análises de exposição de dados.


---

🔍 Principais Operadores de Dorks

1️⃣ Encontrar arquivos específicos

ext:pdf site:gov.br

> Encontra arquivos PDF em sites do governo brasileiro.



ext:xlsx OR ext:csv "lista de emails"

> Procura planilhas que podem conter listas de e-mails.




---

2️⃣ Pesquisar em sites específicos

site:exemplo.com "palavra-chave"

> Busca a palavra-chave apenas dentro do site exemplo.com.



site:exemplo.com filetype:pdf

> Encontra arquivos PDF dentro do site.




---

3️⃣ Localizar diretórios expostos

"Index of /" "parent directory"

> Pode mostrar diretórios abertos em servidores.



"Index of /admin"

> Pode revelar painéis de administração expostos.




---

4️⃣ Buscar câmeras públicas

inurl:/view.shtml

intitle:"Live View / - AXIS"

> Esses comandos podem mostrar câmeras de segurança desprotegidas, mas acessar sem permissão pode ser crime.




---

5️⃣ Achar senhas e credenciais vazadas

"password" filetype:txt

"mysql dump" filetype:sql

> Atenção! O uso indevido dessas informações pode ser ilegal.




---

🛡️ Dorks para Segurança da Informação

Se você deseja verificar se o seu próprio site possui falhas, utilize dorks para identificar arquivos sensíveis expostos:

site:meusite.com filetype:log

> Procura logs expostos.



site:meusite.com inurl:admin

> Busca páginas de administração.




---

# 📌 Dicas de Uso

✅ Combine operadores:

site:exemplo.com intext:"login"

> Encontra páginas que contenham "login" dentro de um site específico.



✅ Use aspas ("") para buscas exatas:

"frase exata"

> Faz a busca exatamente como está escrita.



✅ Evite acessar páginas suspeitas!
Se encontrar algo sensível, não tente explorar. O ideal é relatar ao responsável pela segurança do site.


---

📢 Contribuições

Se quiser adicionar mais dorks úteis, sinta-se à vontade para abrir um Pull Request ou sugerir melhorias na seção de Issues! 🚀


---

📜 Licença

Este repositório é de uso livre para fins educativos e de pesquisa. Não nos responsabilizamos pelo uso indevido das informações aqui contidas.


---
