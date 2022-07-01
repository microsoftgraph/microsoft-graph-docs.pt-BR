---
title: Migrar o Graph do Azure Active Directory (Azure AD) para o Microsoft Graph
description: Saiba como migrar aplicativos do Graph do Azure Active Directory (Azure AD) para o Microsoft Graph antes que Azure AD Graph seja desativado.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 12e080c58217a159d011a14a854f1bab3456f5fc
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577753"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Migrar aplicativos Azure AD Graph para o Microsoft Graph

> [!IMPORTANT]
> O Graph do Azure Active Directory (Azure AD) foi preterido, mas não será desativado em 30 de junho de 2022, conforme anunciado [anteriormente](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363). Ouvindo com atenção seus comentários sobre os desafios de migrar uma dependência tão crítica, estamos atrasando a data de desativação até pelo menos o final deste ano de 2022. Forneceremos uma atualização de desativação no meio do ano civil, incluindo a liberação de mais ferramentas para ajudá-lo a migrar seus aplicativos.

## <a name="why-use-microsoft-graph"></a>Por que usar o Microsoft Graph?

O Microsoft Graph representa nossa melhor superfície de API. Ele oferece um único ponto de extremidade unificado para acessar Azure AD serviços e serviços do Microsoft 365, como o Microsoft Teams e o Microsoft Intune. O API do Graph da Microsoft duplicou o uso do Azure AD Graph e, nos últimos dois anos, adicionamos [167 novos recursos](https://developer.microsoft.com/en-us/graph/changelog). Todas as novas funcionalidades só estarão disponíveis por meio do Microsoft Graph.

O Microsoft Graph também é mais seguro e resiliente do que Azure AD Graph.

O Microsoft Graph tem todos os recursos que estão disponíveis no Azure AD Graph e novas APIs, como métodos de autenticação e proteção de identidade. Suas bibliotecas de clientes oferecem suporte interno para recursos como tratamento de repetição, redirecionamentos seguros, autenticação transparente e compactação de conteúdo.

Alterne para o Microsoft Graph para aproveitar esses recursos avançados e:

- [Gerenciamento de grupos do Microsoft 365](/graph/office365-groups-concept-overview).
- [Convites de usuário externo](/graph/api/resources/invitation).
- A capacidade de [restaurar usuários, grupos, aplicativos e entidades de serviço do Microsoft 365](/graph/api/resources/directory) depois que eles forem excluídos.
- [Notificações de webhook em usuários e grupos](/graph/webhooks).
- Recursos avançados de gerenciamento de licenças, incluindo [licenciamento baseado em grupo](/graph/api/group-assignlicense).
- Recursos de governança de identidade, como:
  - [PIM (Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root) ) para elevar os usuários a funções privilegiadas somente quando necessário e por um período limitado.
  - [Revisões de acesso](/graph/api/resources/accessreviewsv2-overview) para revisões de acesso única ou recorrentes para atestado dos direitos de acesso do usuário.
  - [Termos de uso para permitir que](/graph/api/resources/agreement) as organizações apresentem informações sobre requisitos legais ou de conformidade, como avisos de isenção de responsabilidade.
- Recursos de segurança como:
  - [Eventos de risco de identidade](/graph/api/resources/riskdetection).
  - [Usuários arriscados](/graph/api/resources/riskyuser).
- [Bibliotecas de cliente e exemplos](/graph/) disponíveis em muito mais plataformas e linguagens. Os SDKs do Microsoft Graph fornecem uma interface detectável para acessar facilmente seus dados enquanto manipulam de forma transparente a aquisição de token, tratamento de repetição devido a erros e limitação, tratamento de redirecionamento seguro e serialização e desserialização de modelo.
- Mais [recursos de consulta OData](/graph/query-parameters) compatíveis com recursos como usuários, grupos, aplicativos e entidades de serviço.

O restante dos artigos nesta seção ajuda você a migrar seu aplicativo do Azure AD Graph para o Microsoft Graph. Você encontrará:

- Uma lista de verificação para ajudá-lo a planejar a migração.
- Diretrizes que descrevem diferenças específicas entre as APIs.
- Links para mais recursos e exemplos para ilustrar diferenças específicas.
- Perguntas frequentes para resolver outras perguntas ou preocupações.

Envie outras perguntas, problemas abertos e solicitações de recursos por meio do Microsoft Q&A usando a marca [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html).

## <a name="next-steps"></a>Próximos passos

- Percorra a lista [de verificação de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md) para ajudá-lo a planejar a migração.
- Explore [os conceitos](/graph/overview) e as práticas do Microsoft Graph.
- Use [o Explorador do Graph](https://aka.ms/ge) para experimentar com o Microsoft Graph.
- Saiba mais sobre atualizações de progresso e linhas do tempo [no Microsoft Graph ou no Azure AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/).
- Obtenha [respostas para perguntas que](/graph/migrate-azure-ad-graph-faq) você pode ter sobre a migração.