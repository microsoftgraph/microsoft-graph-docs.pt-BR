---
title: Perfis de publicação no local
description: Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3774ceb0a2e03b8c625bf317467c670c93596ac9
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556237"
---
# <a name="on-premises-publishing-profiles"></a>Perfis de publicação no local

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Vários serviços do Azure (por exemplo, a autenticação de [passagem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)do Azure Active Directory Connect, o [WORKDAY para o provisionamento de usuários do Azure ad](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [proxy de aplicativo](https://aka.ms/whyappproxy) permitem o acesso a vários recursos locais de fora da rede corporativa. [Os agentes locais](onpremisesagent.md) (ou [conectores](connector.md) para o proxy de aplicativo) instalados por um administrador de locatários podem ser configurados para rotear solicitações para um determinado [recurso publicado](publishedresource.md).
Os [grupos de agentes](onpremisesagentgroup.md) (ou grupos de [conectores](connectorgroup.md) para o proxy de aplicativo) permitem que um administrador de locatários atribua agentes específicos para atender a recursos específicos publicados no local. Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo. Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo [onPremisesPublishingProfile](onpremisespublishingprofile.md).

Um administrador de locatários pode configurar para cada **onPremisesPublishingProfile** a [janela de tempo](updatewindow.md) durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes. A [configuração de atualizador](hybridagentupdaterconfiguration.md) especificada para um **onPremisesPublishingProfile** é aplicável a todos os agentes dentro desse **onPremisesPublishingProfile**.

## <a name="see-also"></a>Confira também

- [Agente local](onpremisesagent.md)
- [Grupo de agentes local](onpremisesagentgroup.md)
- [Perfil de publicação local](onpremisespublishingprofile.md)
- [Recurso publicado](publishedresource.md)
- [Connector](connector.md)
- [Grupo de conectores](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
