# Falatuga

Ferramenta gratuita que adapta currículos de português do Brasil para português europeu, para quem procura emprego em Portugal.

2026 · Produto próprio · 🟡 Em desenvolvimento · falatuga.pt

## O problema

Um currículo escrito em português do Brasil carrega vocabulário, formato e termos que não fazem sentido em Portugal. Quem chega para procurar emprego perde pontos antes mesmo da entrevista, sem ter como saber sozinho o que precisa trocar.

## O que construí até agora

- Cola o currículo ou envia PDF e Word em PT-BR, recebe a versão em PT-PT
- Mostra antes e depois, lista as palavras trocadas, exporta em PDF e Word
- Glossário próprio com 451 termos, em três modos: troca automática, sugestão para termos ambíguos (presunto, fato, piso, demissão) e apenas orientação ao modelo para termos como "time"
- Antes de enviar ao modelo, o código apaga CPF e RG e protege siglas que não podem mudar (COREN, CRM, OAB, SUS, UBS, CLT...)
- Depois da resposta, restaura os termos protegidos, remove NIF inventado pelo modelo e aplica o glossário
- 5 currículos de teste aprovados (TI, barbeiro, enfermeira, vendedor, cozinheira), 10 a 20 segundos cada

## Por que as regras ficam no código

A AMÁLIA (9B parâmetros) reescreve bem, mas segue mal instruções do tipo "não faça X". As regras críticas viraram código testado, em vez de instrução de prompt.

## Modelo

Gratuito para quem usa. Roda num Hugging Face Space público com GPU gratuita (ZeroGPU). Grant comunitário solicitado ao Hugging Face.

## Stack

Next.js · JavaScript · Tailwind · shadcn/ui · Supabase · Vercel

## Meu papel

Produto, prompt engineering, arquitetura e implementação. Sozinho, com o Claude Code e Codex.

Projeto independente, sem afiliação ao consórcio AMÁLIA nem ao Governo de Portugal. Feito pelo criador do Tapinfy.
