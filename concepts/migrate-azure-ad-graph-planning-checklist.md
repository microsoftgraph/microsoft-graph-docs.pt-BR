---
title: Lista de verificação de planejamento de migração de aplicativos
description: Lista de verificação para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 5470366e3b61cde18b52246483a46485f3f00c68
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288661"
---
# <a name="app-migration-planning-checklist"></a>Lista de verificação de planejamento de migração de aplicativos

> [!Important]
> A API do Azure AD Graph já foi preterida. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas não fornecerá mais atualizações de recurso.
> A partir de 30 de junho de 2022, encerraremos o suporte para o Azure AD Graph e não fornecerá mais suporte técnico ou atualizações de segurança. Os aplicativos que usam o Azure AD Graph após esse momento não receberão mais respostas do ponto de extremidade do Azure AD Graph.

Use a lista de verificação a seguir para planejar sua migração.

## <a name="step-1-review-the-differences-between-the-apis"></a>Etapa 1: revise as diferenças entre as APIs

Em muitos aspectos, o Microsoft Graph é semelhante ao gráfico do Azure AD anterior. Em muitos casos, basta alterar o nome e a versão do serviço de ponto de extremidade no seu código, e tudo deve continuar a funcionar.

No entanto, há diferenças. Determinados recursos, propriedades, métodos e recursos principais foram alterados.

Especificamente, procure as diferenças nas seguintes áreas:

- [Solicitar sintaxe de chamada](migrate-azure-ad-graph-request-differences.md) entre os dois serviços
- [Diferenças de recursos](migrate-azure-ad-graph-feature-differences.md), como extensões de diretório, processamento em lotes, consultas diferenciais e assim por diante
- [Nomes de recursos de entidade](migrate-azure-ad-graph-resource-differences.md) e seus tipos
- [Propriedades](migrate-azure-ad-graph-property-differences.md) de objetos de solicitação e resposta
- [Métodos](migrate-azure-ad-graph-method-differences.md), incluindo parâmetros e tipos

## <a name="step-2-examine-api-use"></a>Etapa 2: examinar o uso da API

[Examine as APIs](migrate-azure-ad-graph-audit-api-use.md) usadas por seu aplicativo, as permissões necessárias e compare com a lista de diferenças conhecidas.  

Verifique se as APIs de que seu aplicativo precisa estão geralmente disponíveis no Microsoft Graph v 1.0 e se essas APIs funcionam da mesma maneira.

Em alguns casos, novos recursos e recursos foram projetados para substituir as abordagens anteriores.

Use o [Explorador do Graph](https://aka.ms/ge) para experimentar novas chamadas e desenvolver novas abordagens. Para obter melhores resultados, entre usando as credenciais de um usuário de teste em um locatário de teste para ver o que a API faz sobre conjuntos de dados importantes.

## <a name="step-3-review-app-details"></a>Etapa 3: examinar os detalhes do aplicativo

- Alterações de consentimento e [registro de aplicativo](migrate-azure-ad-graph-app-registration.md) (que devem ser nenhuma).
- Aquisição de token e [bibliotecas de autenticação](migrate-azure-ad-graph-authentication-library.md).
- Para aplicativos .NET, use de [bibliotecas de cliente](migrate-azure-ad-graph-client-libraries.md).

## <a name="step-4-deploy-test-and-extend-your-app"></a>Etapa 4: implantar, testar e estender seu aplicativo

Antes de atualizar seu aplicativo para todos, assegure-se de testar cuidadosamente e preparar sua distribuição para o público do cliente.

Agora você já fez a migração para o Microsoft Graph, nunca foi mais fácil desbloquear muito mais conjuntos de informações e recursos que agora estão em suas mãos. Você pode ter uma idéia do que é possível examinando alguns [exemplos](/graph/examples).

Se você estiver usando a [biblioteca de autenticação do AD](/azure/active-directory/develop/active-directory-authentication-libraries) (Adal), considere mudar para a biblioteca de autenticação da [Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL).

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre a [solicitação de sintaxe de chamada](migrate-azure-ad-graph-request-differences.md) para iniciar a etapa 1: revisando as diferenças da API.