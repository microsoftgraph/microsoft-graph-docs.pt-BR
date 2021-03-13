---
title: Lista de verificação de planejamento de migração de aplicativos
description: Lista de verificação para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: a61e5180194246bbea5cc32e42666beab83882fa
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761280"
---
# <a name="app-migration-planning-checklist"></a>Lista de verificação de planejamento de migração de aplicativos

> [!Important]
> A API do Azure AD Graph agora está preterida. Continuaremos dando suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.
> A partir de 30 de junho de 2022, encerraremos o suporte para o Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança. Os aplicativos que usam o Azure AD Graph após esse tempo não receberão mais respostas do ponto de extremidade do Azure AD Graph.

Use a lista de verificação a seguir para planejar sua migração.

## <a name="step-1-review-the-differences-between-the-apis"></a>Etapa 1: Analisar as diferenças entre as APIs

Em muitos aspectos, o Microsoft Graph é semelhante ao Gráfico do Azure AD anterior. Em muitos casos, basta alterar o nome e a versão do serviço de ponto de extremidade em seu código e tudo deve continuar a funcionar.

No entanto, há diferenças. Determinados recursos, propriedades, métodos e recursos principais foram alterados.

Especificamente, procure diferenças nas seguintes áreas:

- [Solicitar sintaxe de chamada](migrate-azure-ad-graph-request-differences.md) entre os dois serviços
- [Diferenças de](migrate-azure-ad-graph-feature-differences.md)recursos , como extensões de diretório, lotes, consultas diferenciais e assim por diante
- [Nomes de recursos de entidade](migrate-azure-ad-graph-resource-differences.md) e seus tipos
- [Propriedades](migrate-azure-ad-graph-property-differences.md) de objetos de solicitação e resposta
- [Métodos](migrate-azure-ad-graph-method-differences.md), incluindo parâmetros e tipos

## <a name="step-2-examine-api-use"></a>Etapa 2: Examinar o uso da API

[Examine as APIs](migrate-azure-ad-graph-audit-api-use.md) usadas pelo seu aplicativo, as permissões necessárias e compare com a lista de diferenças conhecidas.  

Verifique se as APIs que seu aplicativo precisa estão geralmente disponíveis no Microsoft Graph v1.0 e se essas APIs funcionam da mesma maneira.

Em alguns casos, novos recursos e recursos são projetados para substituir abordagens anteriores.

Use o [Explorador do Graph](https://aka.ms/ge) para experimentar novas chamadas e desenvolver novas abordagens. Para melhores resultados, entre usando as credenciais de um usuário de teste em um locatário de teste para que você veja o que a API faz em conjuntos de dados importantes.

## <a name="step-3-review-app-details"></a>Etapa 3: Revisar detalhes do aplicativo

- [Alterações de registro e](migrate-azure-ad-graph-app-registration.md) consentimento do aplicativo (que não devem ser nenhuma).
- Bibliotecas de autenticação e aquisição [de tokens.](migrate-azure-ad-graph-authentication-library.md)
- Para aplicativos .NET, use [bibliotecas de clientes.](migrate-azure-ad-graph-client-libraries.md)

## <a name="step-4-deploy-test-and-extend-your-app"></a>Etapa 4: Implantar, testar e estender seu aplicativo

Antes de atualizar seu aplicativo para todos, verifique se você testou completamente e estágiou sua lançamento para o público-alvo.

Agora que você alternou para o Microsoft Graph, nunca foi mais fácil desbloquear muitos mais conjuntos de dados e recursos que agora estão à sua ponta dos dedos. Você pode obter uma amostra do que é possível analisando alguns dos principais serviços [e recursos no Microsoft Graph.](./overview-major-services.md)

Se você estiver usando a biblioteca de autenticação [do AD (ADAL),](/azure/active-directory/develop/active-directory-authentication-libraries) considere alternar para a biblioteca de autenticação da [Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL).

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre a sintaxe de chamada de](migrate-azure-ad-graph-request-differences.md) solicitação para iniciar a etapa 1: analisar as diferenças de API.