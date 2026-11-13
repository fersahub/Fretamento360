# Fretamento360

Aplicação web demonstrativa para gestão operacional de transporte fretado.

## Demonstração

A versão inicial é um frontend estático em `public/`, pronto para GitHub Pages. O app disponibiliza dashboard, diagnóstico operacional, ocorrências, quebras e atrasos, programação, escalas, frota, motoristas, rotas, SLA, relatórios CSV e procedimentos.

## Publicação automática

1. No repositório, abra **Settings → Pages**.
2. Em **Build and deployment → Source**, selecione **GitHub Actions**.
3. Acesse **Actions** e acompanhe a execução do workflow **Publicar Fretamento360 no GitHub Pages**.
4. Após a execução bem-sucedida, acesse https://fersahub.github.io/Fretamento360/.

A publicação é disparada por alterações na pasta `public/` ou no workflow.

## Dados e segurança

Esta primeira versão usa dados demonstrativos gravados no armazenamento local do navegador (`localStorage`). Os registros não são sincronizados entre computadores ou usuários. Não insira dados reais ou pessoais de motoristas e passageiros. Antes do uso operacional, será necessário implementar backend, autenticação, banco de dados, controle de acesso, backups e políticas de privacidade.

O índice de SLA é apenas ilustrativo; configure critérios contratuais antes de usá-lo em relatórios oficiais.

## Desenvolvimento futuro

A próxima etapa será conectar o frontend a um backend Supabase com autenticação, banco de dados e regras de acesso. O GitHub Pages hospeda apenas arquivos estáticos e não substitui o backend.
