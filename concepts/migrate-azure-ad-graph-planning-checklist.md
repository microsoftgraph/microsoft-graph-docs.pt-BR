---
title: Lista de verificação de planejamento de migração de aplicativos
description: Lista de verificação para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: f8e231166fdb39676ce2778b369c6962cae70cb0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882742"
---
# <a name="app-migration-planning-checklist"></a>Lista de verificação de planejamento de migração de aplicativos

> [!Important]
> A API do Azure AD Graph agora foi preterida. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.
> A partir de 30 de junho de 2022, encerraremos o suporte ao Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança. Os aplicativos que usam o Azure AD Graph após esse período não receberão mais respostas do ponto de extremidade do Azure AD Graph.

Use a lista de verificação a seguir para planejar sua migração.

## <a name="step-1-review-the-differences-between-the-apis"></a>Etapa 1: Revise as diferenças entre as APIs

Em muitos aspectos, o Microsoft Graph é semelhante ao Azure AD Graph anterior. Em muitos casos, basta alterar o nome e a versão do serviço de ponto de extremidade em seu código, e tudo deve continuar a funcionar.

No entanto, há diferenças. Determinados recursos, propriedades, métodos e recursos principais foram alterados.

Especificamente, procure diferenças nas seguintes áreas:

- [Sintaxe de chamada de solicitação](migrate-azure-ad-graph-request-differences.md) entre os dois serviços
- [Diferenças de](migrate-azure-ad-graph-feature-differences.md)recursos, como extensões de diretório, processamento em lotes, consultas diferenciais e assim por diante
- [Nomes de recursos de entidade](migrate-azure-ad-graph-resource-differences.md) e seus tipos
- [Propriedades de](migrate-azure-ad-graph-property-differences.md) objetos de solicitação e resposta
- [Métodos,](migrate-azure-ad-graph-method-differences.md)incluindo parâmetros e tipos

## <a name="step-2-examine-api-use"></a>Etapa 2: Examinar o uso da API

[Examine as APIs](migrate-azure-ad-graph-audit-api-use.md) usadas pelo seu aplicativo, as permissões necessárias e compare com a lista de diferenças conhecidas.  

Verifique se as APIs de que seu aplicativo precisa estão geralmente disponíveis no Microsoft Graph v1.0 e se essas APIs funcionam da mesma maneira.

Em alguns casos, novos recursos são projetados para substituir abordagens anteriores.

Use o [Explorador do Graph](https://aka.ms/ge) para experimentar novas chamadas e desenvolver novas abordagens. Para melhores resultados, entre usando as credenciais de um usuário de teste em um locatário de teste para que você veja o que a API faz em conjuntos de dados importantes.

## <a name="step-3-review-app-details"></a>Etapa 3: Analisar detalhes do aplicativo

- [Alterações de registro e](migrate-azure-ad-graph-app-registration.md) consentimento do aplicativo (que não devem ser nenhuma).
- Bibliotecas de [aquisição e autenticação de tokens.](migrate-azure-ad-graph-authentication-library.md)
- Para aplicativos .NET, uso de [bibliotecas de cliente.](migrate-azure-ad-graph-client-libraries.md)

## <a name="step-4-deploy-test-and-extend-your-app"></a>Etapa 4: Implantar, testar e estender seu aplicativo

Antes de atualizar seu aplicativo para todos, teste exaustivamente e teste sua lançamento para o público-alvo.

Agora que você alternou para o Microsoft Graph, nunca foi mais fácil desbloquear muito mais conjuntos de dados e recursos que agora estão ao seu alcance. Você pode ter uma amostra do que é possível observando alguns dos principais serviços [e recursos do Microsoft Graph.](./overview-major-services.md)

Se você estiver usando a biblioteca de autenticação do [AD (ADAL),](/azure/active-directory/develop/active-directory-authentication-libraries) considere mudar para a biblioteca de autenticação da [Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL).

## <a name="next-steps"></a>Próximas Etapas

- Saiba mais sobre [a sintaxe de chamada de](migrate-azure-ad-graph-request-differences.md) solicitação para iniciar a etapa 1: analisar as diferenças da API.