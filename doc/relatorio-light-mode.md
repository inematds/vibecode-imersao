# REVISAO DO CURSO: Imersao Vibe Coding
## Foco: Temas e Cores (Dark/Light Mode)

**Data:** 2026-03-11
**Arquivos analisados:** 49
**Problemas encontrados:** 12 categorias afetando todos os 49 arquivos

---

## CRITICO (7):

### 1. Body com gradiente no light mode (49 arquivos)
- Todos usam `background: linear-gradient(135deg, #f8fafc 0%, #e2e8f0 50%, #f1f5f9 100%)`
- **Deveria ser:** `background-color: #f8fafc` (cor solida)
- **Impacto:** Fundo irregular, visual "sujo" em telas grandes

### 2. Cores de acento da trilha SEM override light mode (48 arquivos)
- Classes como `text-emerald-400`, `text-blue-400`, `text-purple-400`, `text-amber-400`, `text-teal-400`, `text-rose-400` ficam com as cores do dark mode (claras/neon) sobre fundo branco
- **Impacto GRAVE:** Texto emerald-400/teal-400/amber-400 tem contraste PESSIMO contra fundo branco. Amarelo e verde claro sobre branco = quase invisivel
- **Faltam 5 regras por cor por trilha:**
  - `html:not(.dark) .text-COR-400 { color: VALOR_ESCURO; }`
  - `html:not(.dark) .bg-COR-500\/20 { ... }`
  - `html:not(.dark) .bg-COR-500\/10 { ... }`
  - `html:not(.dark) .border-COR-500\/30 { ... }`
  - `html:not(.dark) .hover\:bg-COR-500\/30:hover { ... }`

### 3. Cor `text-primary` (#FACC15 = amarelo) sem override (49 arquivos)
- Amarelo vivo sobre fundo branco = ilegivel
- Usado em "Conceitos-chave", CTAs, dicas - elementos importantes ficam invisiveis
- ~25 ocorrencias por modulo
- **Deveria ser:** `color: #a16207` (amber escuro)

### 4. Cor `text-yellow-400` sem override (49 arquivos)
- Logo "Imersao Vibe Coding" na navbar fica amarelo sobre branco = invisivel
- **Deveria ser:** `color: #a16207`

### 5. Cor `text-sky-400` sem override (49 arquivos)
- Link "INEMA.CLUB" na navbar fica azul claro, contraste insuficiente
- **Deveria ser:** `color: #0369a1`

### 6. Gradientes nao removidos no light mode (todos os modulos)
- Classes `bg-gradient-to-br from-COR-900/30 via-dark-800 to-dark-800` ficam com cores escuras no light mode, criando manchas escuras em fundo claro
- ~8 gradientes por modulo (secoes de topicos)
- **Falta:** `html:not(.dark) [class*="bg-gradient-to"] { background-image: none !important; }`

### 7. Navbar sem override de transparencia (49 arquivos)
- `bg-dark-900/95` fica com override para `#ffffff`, mas falta o override especifico de opacidade
- **Falta:** `html:not(.dark) .bg-dark-900\/95 { background-color: rgba(255, 255, 255, 0.95); }`

---

## AVISO (3):

### 8. Landing page (index.html) sem overrides das 6 cores
- A index principal usa TODAS as 6 cores de trilha nos cards mas nao tem override de nenhuma
- Precisa de overrides para emerald, blue, purple, amber, teal E rose + hovers

### 9. `hover:text-sky-300` e `hover:text-yellow-300` sem override (49 arquivos)
- Estados hover da navbar ficam com cores claras no light mode
- **Faltam:** overrides para hover de sky e yellow

### 10. `bg-primary/10` e `border-primary/40` sem override (modulos)
- Backgrounds e bordas das caixas de "Conceitos-chave" ficam com tons amarelos quase invisiveis
- **Faltam:** overrides com tons amber escuros

---

## SUGESTAO (2):

### 11. Considerar sombras suaves nos cards em light mode
- Os cards com `bg-dark-800` ficam com fundo `#f9fafb` que mal se distingue do body `#f8fafc`
- Uma `box-shadow` sutil ajudaria a separar visualmente

### 12. Toggle button styling
- O botao de toggle usa `bg-dark-700` que fica `#f3f4f6` no light mode - funcional, mas poderia ter borda para melhor visibilidade

---

## RESUMO DOS VALORES CORRETOS PARA LIGHT MODE

| Classe dark mode | Valor light mode correto |
|---|---|
| `text-emerald-400` | `#059669` |
| `text-blue-400` | `#2563eb` |
| `text-purple-400` | `#7c3aed` |
| `text-amber-400` | `#92400e` |
| `text-teal-400` | `#0d9488` |
| `text-rose-400` | `#9f1239` |
| `text-primary` | `#a16207` |
| `text-yellow-400` | `#a16207` |
| `text-sky-400` | `#0369a1` |
| body background | `#f8fafc` (solido) |
| navbar bg | `rgba(255,255,255,0.95)` |
| gradientes | `background-image: none !important` |
