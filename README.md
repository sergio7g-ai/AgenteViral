# Viral Content Command Center

Painel HTML para gerir conteúdos, tendências e aprovações usando Supabase.

## Estado atual
- Autenticação Supabase por email/palavra-passe.
- Dashboard de conteúdos, tendências, agenda e histórico.
- Rascunhos e aprovação/rejeição de conteúdos.
- Aprovar um conteúdo não o publica. A publicação social está deliberadamente desligada.
- A pesquisa diária com Claude, as Edge Functions e o agendamento 24/7 ainda precisam de configuração.

## Publicação
Publica o repositório como site estático com GitHub Pages ou Netlify. A chave Supabase publishable pode ser usada no frontend com RLS corretamente configurado. Nunca colocar chaves Anthropic ou tokens de redes sociais no HTML.

## Próximas etapas
1. Configurar um secret da Anthropic no backend.
2. Implementar Edge Function para pesquisa de tendências e geração de rascunhos.
3. Configurar execução diária no backend.
4. Implementar aprovação ligada à versão exata do conteúdo.
5. Ligar APIs oficiais das redes sociais apenas depois de configurar credenciais seguras e testar.

## Segurança
As tabelas usam Row Level Security. A chave publishable não substitui as políticas de acesso.