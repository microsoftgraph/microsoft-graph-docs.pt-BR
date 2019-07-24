---
title: Perfis de publicação no local
description: Vários serviços do Azure (por exemplo, Azue Active Directory Connect PassThrough Authentication, workday to Azure AD Users Provisioning) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9b0e975d932226adfa2c455baaa396c1d580f6ff
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841329"
---
# <a name="on-premises-publishing-profiles"></a>Perfis de publicação no local

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Vários serviços do Azure (por exemplo, Azue Active Directory Connect PassThrough Authentication, workday to Azure AD Users Provisioning) permitem um acesso condicional a vários recursos locais de fora da rede corporativa. [Os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.
Os [grupos de agentes](onpremisesagentgroup.md) permitem que um administrador de locatários atribua agentes específicos para atender recursos locais publicados específicos. Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo. Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo [onPremisesPublishingProfile](onpremisespublishingprofile.md).

Um administrador de locatários pode configurar para cada **onPremisesPublishingProfile** a [janela de tempo](updatewindow.md) durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes. A [configuração](hybridagentupdaterconfiguration.md) de atualizador especificada para um **onPremisesPublishingProfile** é aplicável a todos os agentes dentro desse **onPremisesPublishingProfile**.

## <a name="see-also"></a>Confira também

- [Agente local](onpremisesagent.md)
- [Grupo de agentes local](onpremisesagentgroup.md)
- [Perfil de publicação local](onpremisespublishingprofile.md)
- [Recurso publicado](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
