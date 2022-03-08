---
title: Migrar aplicativos do Azure AD Graph microsoft Graph
description: Descreve como migrar aplicativos de API Azure Active Directory (Azure AD) para a API Graph Microsoft.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: a59b32d7c042d7a6300abb97dc602700a769d3cf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333838"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Migrar aplicativos do Azure AD Graph microsoft Graph

> [!IMPORTANT]
> Azure Active Directory (Azure AD) Graph está preterido, mas não será retirado em 30 de junho de 2022, conforme anunciado [anteriormente](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363). Escutando seus comentários sobre os desafios de migrar uma dependência tão crítica, estamos atrasando a data de aposentadoria até pelo menos o final deste ano, 2022. Forneceremos uma atualização de aposentadoria no meio do ano, incluindo a liberação de mais ferramentas para ajudá-lo a migrar seus aplicativos.

## <a name="why-use-microsoft-graph"></a>Por que usar o Microsoft Graph?

O Microsoft Graph representa nossa melhor superfície de API. Ele oferece um único ponto de extremidade unificado para acessar serviços do Azure AD e serviços Microsoft 365 como Microsoft Teams e Microsoft Intune. O Graph da API da Microsoft duplicou mais do que o uso do Azure AD Graph e, nos últimos dois anos, adicionamos [167 novos recursos](https://developer.microsoft.com/en-us/graph/changelog). Todas as novas funcionalidades só estarão disponíveis por meio do microsoft Graph.

O Microsoft Graph também é mais seguro e resiliente do que o Azure AD Graph.

O Microsoft Graph tem todos os recursos disponíveis no Azure AD Graph e novas APIs, como a proteção de identidade e os métodos de autenticação. Suas bibliotecas de clientes oferecem suporte integrado para recursos como manipulação de nova tentativa, redirecionamentos seguros, autenticação transparente e compactação de carga.

Alternar para o Microsoft Graph para tirar proveito desses recursos avançados e:

- [Microsoft 365 gerenciamento de grupo](/graph/office365-groups-concept-overview).
- [Convites de usuário externos](/graph/api/resources/invitation).
- A capacidade de [restaurar usuários, Microsoft 365 grupos, aplicativos e entidades de serviço](/graph/api/resources/directory) após a exclusão.
- [Notificações de webhook em usuários e grupos](/graph/webhooks).
- Recursos avançados de gerenciamento de licenças, incluindo [licenciamento baseado em grupo](/graph/api/group-assignlicense).
- Recursos de governança de identidade, como:
  - [PiM (gerenciamento de](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) identidade privilegiada) para elevar os usuários a funções privilegiadas somente quando necessário e por um período limitado.
  - [Acesse análises de](/graph/api/resources/accessreviewsv2-overview) acesso para análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário.
  - [Termos de uso para permitir que](/graph/api/resources/agreement) as organizações apresentem informações para requisitos legais ou de conformidade, como avisos de isenção de responsabilidade.
- Recursos de segurança como:
  - [Eventos de risco de identidade](/graph/api/resources/riskdetection).
  - [Usuários arriscados](/graph/api/resources/riskyuser).
- [Bibliotecas de clientes e exemplos](/graph/) disponíveis em muitas outras plataformas e idiomas. Os SDKs do Microsoft Graph fornecem uma interface descobrivel para acessar facilmente seus dados enquanto manipulam de forma transparente a aquisição de tokens, a manipulação de novo devido a erros e a throttling, tratamento seguro de redirecionamento e serialização de modelo e dessarialização.
- Mais [recursos de consulta OData suportados](/graph/query-parameters) por recursos como usuários, grupos, aplicativos e entidades de serviço.

O restante dos artigos nesta seção ajudam você a migrar seu aplicativo do Azure AD Graph para o Microsoft Graph. Você encontrará:

- Uma lista de verificação para ajudá-lo a planejar a migração.
- Diretrizes que descrevem diferenças específicas entre as APIs.
- Links para mais recursos e exemplos para ilustrar diferenças específicas.
- Uma perguntas frequentes para resolver outras perguntas ou preocupações.

Envie outras perguntas, problemas abertos e solicitações de recursos por meio do Microsoft Q&A usando a marca [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html).

## <a name="next-steps"></a>Próximas etapas

- Ande pela lista [de verificação de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md) para ajudá-lo a planejar a migração.
- Explore [os Graph](/graph/overview) e práticas da Microsoft.
- Use [Graph Explorer](https://aka.ms/ge) para experimentar com o Microsoft Graph.
- Para saber mais sobre atualizações de progresso e cronogramas, consulte [Microsoft Graph ou o Azure AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/).
- Obter [respostas para perguntas](/graph/migrate-azure-ad-graph-faq) que você pode ter sobre a migração.