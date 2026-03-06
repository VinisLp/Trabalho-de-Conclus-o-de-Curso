# Arquitetura do UrbApp

## Visão Geral

O sistema será dividido em três camadas principais:

1. **Cliente Móvel**
   - Framework sugerido: React Native ou Flutter.
   - Responsável por exibir mapa, formulários de report e perfil de usuário.

2. **APIs / Backend**
   - Servidor RESTful (Node.js/Express, Django, etc.).
   - Endpoints para autenticação, criação/listagem de reports, gamificação.
   - Atenção especial a controle de acesso e validação de dados.

3. **Banco de Dados**
   - PostgreSQL com extensão PostGIS para queries geoespaciais.
   - Tabelas principais: `users`, `reports`, `points`, `badges`.

## Componentes auxiliares

- **Serviço de geocodificação** (reverse geocoding ao criar report).
- **Sistema de notificação push** para informar usuário sobre validações e conquistas.
- **Integração com API de mapas** (OpenStreetMap ou Google Maps SDK).

## Fluxo básico**

1. Usuário se autentica no app.
2. Cadastra report: foto, descrição e localização.
3. Backend valida e salva no DB, calcula pontos.
4. Cliente atualiza UI e mostra nova pontuação.
5. Administrador revisa e publica report.

