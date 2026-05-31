# Guia: char* e String em C

Guia completo e didático sobre manipulação de strings em C/C++ embarcado, pronto para publicar no **GitHub Pages**.

É um site estático de arquivo único (`index.html`) — sem build, sem dependências, sem framework. Abra localmente ou publique direto.

---

## Visualizar localmente

Basta abrir o arquivo no navegador:

```bash
# Opção 1 — abrir direto
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows

# Opção 2 — servidor local (recomendado)
python3 -m http.server 8000
# acesse http://localhost:8000
```

---

## Publicar no GitHub Pages

### Passo a passo

1. **Crie um repositório** no GitHub (ex: `guia-strings-c`).

2. **Envie os arquivos:**

```bash
git init
git add index.html README.md
git commit -m "Guia char* e String em C"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/guia-strings-c.git
git push -u origin main
```

3. **Ative o GitHub Pages:**
   - No repositório, vá em **Settings → Pages**
   - Em **Source**, selecione a branch **main** e a pasta **/ (root)**
   - Clique em **Save**

4. **Aguarde ~1 minuto.** O site ficará disponível em:
   ```
   https://SEU_USUARIO.github.io/guia-strings-c/
   ```

### Usar um domínio de projeto raiz (opcional)

Se quiser que o guia seja a página principal do seu usuário, nomeie o repositório como `SEU_USUARIO.github.io`. O site ficará em `https://SEU_USUARIO.github.io/`.

---

## Estrutura do conteúdo

O guia tem 11 seções progressivas:

| # | Seção | Foco |
|---|-------|------|
| 01 | O que é uma string em C | Terminador `\0`, strlen vs sizeof |
| 02 | Array de char | String mutável na stack |
| 03 | O ponteiro char* | Literais vs arrays, aritmética de ponteiro |
| 04 | Funções da string.h | strcpy, strcat, strcmp, strchr |
| 05 | Formatação com snprintf | Buffer seguro, especificadores |
| 06 | Erros comuns | Overflow, dangling pointer, terminador |
| 07 | A classe String | API do Arduino |
| 08 | char* vs String | Tabela de decisão |
| 09 | Fragmentação de heap | O perigo do uso intenso de String |
| 10 | Boas práticas | Padrões recomendados, checklist |
| 11 | Conclusão | Síntese e próximos passos |

---

## Personalização

Todo o estilo está em variáveis CSS no topo do `<style>` em `index.html`:

```css
:root{
  --bg:#0e1116;        /* fundo principal */
  --amber:#e8a33d;     /* cor de destaque */
  --cyan:#5fd3c4;      /* cor secundária */
  /* ... */
}
```

Para trocar o esquema de cores, edite apenas esses valores. As fontes (Fraunces, JetBrains Mono, Newsreader) vêm do Google Fonts e podem ser trocadas no `<link>` do `<head>`.

---

## Licença

MIT — use, adapte e compartilhe livremente.
