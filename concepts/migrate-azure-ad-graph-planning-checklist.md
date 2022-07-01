---
title: Lista de verificação de migração de aplicativos do Graph do Azure Active Directory (Azure AD)
description: Use esta lista de verificação para migrar seus aplicativos do Azure Active Directory (Azure AD) Graph para o Microsoft Graph.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: ca3625d7462d1801dc5056f6f65246495aee1e56
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577697"
---
# <a name="azure-ad-graph-app-migration-planning-checklist"></a>Azure AD de verificação de planejamento de migração de aplicativos do Graph

Use a lista de verificação a seguir para planejar sua migração do Azure Active Directory (Azure AD) Graph para o Microsoft Graph.

## <a name="step-1-review-the-differences-between-the-apis"></a>Etapa 1: Examinar as diferenças entre as APIs

Em muitos aspectos, o Microsoft Graph é semelhante ao anterior Azure AD Graph. Em muitos casos, basta alterar o nome e a versão do serviço de ponto de extremidade em seu código, e tudo deve continuar funcionando.

No entanto, há diferenças. Determinados recursos, propriedades, métodos e recursos principais foram alterados.

Especificamente, procure diferenças nas seguintes áreas:

- [Sintaxe de chamada de](migrate-azure-ad-graph-request-differences.md) solicitação entre os dois serviços
- [Diferenças de](migrate-azure-ad-graph-feature-differences.md) recursos, como extensões de diretório, envio em lote, consultas diferenciais e assim por diante
- [Nomes de recursos de entidade](migrate-azure-ad-graph-resource-differences.md) e seus tipos
- [Propriedades de](migrate-azure-ad-graph-property-differences.md) objetos de solicitação e resposta
- [Métodos,](migrate-azure-ad-graph-method-differences.md) incluindo parâmetros e tipos

## <a name="step-2-examine-api-use"></a>Etapa 2: Examinar o uso da API

[Examine as APIs](migrate-azure-ad-graph-audit-api-use.md) usadas pelo seu aplicativo, as permissões necessárias e compare com a lista de diferenças conhecidas.  

Verifique se as APIs de que seu aplicativo precisa estão geralmente disponíveis no Microsoft Graph v1.0 e se essas APIs funcionam da mesma maneira.

Em alguns casos, novos recursos e recursos são projetados para substituir abordagens anteriores.

Use [o Explorador do Graph](https://aka.ms/ge) para experimentar novas chamadas e desenvolver novas abordagens. Para obter melhores resultados, entre usando as credenciais de um usuário de teste em um locatário de teste para que você veja o que a API faz em conjuntos de dados importantes.

## <a name="step-3-review-app-details"></a>Etapa 3: Examinar detalhes do aplicativo

- [Alterações de registro e](migrate-azure-ad-graph-app-registration.md) consentimento do aplicativo (que não devem ser nenhuma).
- Bibliotecas de [autenticação e aquisição de token](migrate-azure-ad-graph-authentication-library.md).
- Para aplicativos .NET, use [bibliotecas de cliente](migrate-azure-ad-graph-client-libraries.md).

## <a name="step-4-deploy-test-and-extend-your-app"></a>Etapa 4: Implantar, testar e estender seu aplicativo

Antes de atualizar seu aplicativo para todos, certifique-se de testar completamente e preparar sua distribuição para o público-alvo do cliente.

Agora que você fez a mudança para o Microsoft Graph, nunca foi mais fácil desbloquear muitos outros conjuntos de dados e recursos que agora estão ao seu alcance. Você pode experimentar o que é possível examinando alguns dos principais serviços [e recursos do Microsoft Graph](./overview-major-services.md).

[A MSAL](/azure/active-directory/develop/reference-v2-libraries) (biblioteca de autenticação da Microsoft) agora é a biblioteca de autenticação recomendada para uso com o plataforma de identidade da Microsoft. Se você estiver usando a ADAL (Biblioteca de Autenticação do [Azure Active Directory](/azure/active-directory/develop/active-directory-authentication-libraries) ), planeje alternar para a MSAL. Consulte mais diretrizes para [migrar aplicativos para a MSAL (Biblioteca](/azure/active-directory/develop/msal-migration) de Autenticação da Microsoft).

## <a name="next-steps"></a>Próximos passos

- Saiba mais [sobre a sintaxe da chamada de](migrate-azure-ad-graph-request-differences.md) solicitação para iniciar a etapa 1: examinar as diferenças de API.
