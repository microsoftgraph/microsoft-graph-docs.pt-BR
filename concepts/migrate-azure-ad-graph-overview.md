---
title: Migrar aplicativos do Azure AD Graph para o Microsoft Graph
description: Descreve como migrar aplicativos de API do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 311bc8c800d7415e7e2d192f5b11aed971faafa4
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926775"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Migrar aplicativos do Azure AD Graph para o Microsoft Graph

O Microsoft Graph está substituindo o gráfico do Azure Active Directory (Azure AD). Para a maioria dos aplicativos de produção, o Microsoft Graph já pode oferecer suporte completo aos cenários do Azure AD. Você deve começar a mover seus aplicativos do Azure AD Graph para o Microsoft Graph agora.

Além disso, o Microsoft Graph oferece suporte a vários novos conjuntos de jogos e recursos do Azure AD que não estão disponíveis no Azure AD Graph. Alterne para o Microsoft Graph para aproveitar essas novas APIs, tudo por meio de um único ponto de extremidade, incluindo:

- [Gerenciamento de grupo do Office 365](/graph/office365-groups-concept-overview)
- [Convites de usuário externo](/graph/api/resources/invitation?view=graph-rest-1.0)
- A capacidade de [restaurar usuários e grupos do Office 365](/graph/api/resources/directory?view=graph-rest-1.0) depois de excluídos
- [Notificações de webhook em usuários e grupos](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
- Recursos de governança de identidade, como:
  - [Gerenciamento de identidade privilegiado](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) para elevar os usuários a funções privilegiadas apenas quando necessário e por um período de tempo limitado
  - [Revisões de acesso](/graph/api/resources/accessreviews-root?view=graph-rest-beta) para avaliações de acesso de um único momento ou recorrentes para atestado dos direitos de acesso do usuário
  - [Termos de uso](/graph/api/resources/accessreviews-root?view=graph-rest-beta) para permitir que as organizações apresentem informações para requisitos legais ou de conformidade, como avisos de isenção de responsabilidade
- Recursos de segurança como:
  - [Eventos de risco de identidade](/graph/api/resources/identityriskevent?view=graph-rest-beta)
  - [Usuários de risco](/graph/api/resources/riskyuser?view=graph-rest-beta)
- [Bibliotecas e exemplos de cliente](/graph/) disponíveis em muitas plataformas e outros idiomas. Os SDKs do Microsoft Graph fornecem uma interface detectável para acessar facilmente seus dados ao lidar com a aquisição de token de forma transparente, tentar novamente o tratamento devido a erros e limitação, tratamento de redirecionamento seguro e serialização e desserialização de modelo.

O Microsoft Graph oferece acesso a muitos outros serviços do que apenas ao Azure Active Directory. Também é o [gateway da API para os serviços do Microsoft 365](/graph/).

O restante dos artigos desta seção o ajudará a mover seu aplicativo do Azure AD Graph para o Microsoft Graph. Você encontrará:

- Uma lista de verificação para ajudá-lo a planejar.
- Orientações que descrevem diferenças específicas entre as APIs.
- Links para recursos adicionais e exemplos para ilustrar diferenças específicas.

## <a name="next-steps"></a>Próximas etapas

- Mostre a [lista de verificação de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md) para ajudá-lo a planejar a movimentação.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
- Para saber mais sobre atualizações de progresso e cronogramas, confira [Microsoft Graph ou o Azure ad Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/).
