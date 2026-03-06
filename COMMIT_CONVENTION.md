# Padrão de Commits - UrbApp

Este documento descreve o padrão de commit adotado no projeto UrbApp.

## Guia de Commits

### Categorias Permitidas

- **Adição**: Quando você adiciona novos arquivos, funcionalidades ou módulos
- **Modificação**: Quando você altera o código existente (melhorias, refatoração)
- **Correção**: Quando você corrige bugs ou problemas

### Formato da Mensagem

```
[Categoria]: [Descrição breve]

[Descrição detalhada - opcional]
```

### Exemplos

#### Adição
```
Adição: Implementar módulo de autenticação

- Criar arquivo de autenticação
- Implementar função de login
- Adicionar validação de token
```

#### Modificação
```
Modificação: Melhorar performance da API

Otimização das queries do banco de dados
reduzindo tempo de resposta em 40%
```

#### Correção
```
Correção: Corrigir bug no formulário de login

O campo de email não validava corretamente
endereços com subdomínios
```

## Boas Práticas

1. ✅ Use mensagens claras e descritivas
2. ✅ Escreva em português ou inglês (escolha um e mantenha consistência)
3. ✅ Mantenha commits pequenos e focados
4. ✅ Revise seu código antes de fazer commit
5. ✅ Inclua referências a issues quando aplicável

## ❌ O que evitar

1. ❌ Mensagens genéricas: "atualizei", "novo arquivo"
2. ❌ Commits muito grandes com múltiplas mudanças
3. ❌ Commits sem quebras de linha
4. ❌ Usar caracteres especiais desnecessários
