---
title: Perfis de publicação local
description: Vários serviços do Azure (por exemplo, a Autenticação de Passagem do Azure Active Directory Connect, o dia de trabalho para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 44d09da274413b23092afea6290c0c32a64f8500
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134873"
---
# <a name="on-premises-publishing-profiles"></a>Perfis de publicação local

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Vários serviços do Azure (por exemplo, a Autenticação de Passagem do Azure Active Directory [Connect,](/azure/active-directory/hybrid/how-to-connect-pta)o dia de trabalho para o provisionamento de usuários do [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [Proxy](https://aka.ms/whyappproxy)  de aplicativo permitem acesso a vários recursos locais de fora da rede corporativa. [Agentes locais (ou](onpremisesagent.md) conectores para Proxy de Aplicativo) instalados por um administrador de locatários podem ser [configurados](connector.md) para encaminhar solicitações para um recurso [publicado específico.](publishedresource.md)
[Grupos de agentes](onpremisesagentgroup.md) (ou [grupos de](connectorgroup.md) conectores para Proxy de Aplicativo) permitem que um administrador de locatários atribua agentes específicos para atender a recursos locais publicados específicos. Os administradores de locatários podem agrupar vários agentes e atribuir cada recurso publicado a um grupo. Todo o conjunto de entidades do mesmo tipo de publicação local é representado por [onPremisesPublishingProfile](onpremisespublishingprofile.md).

Um administrador de locatários pode configurar para [](updatewindow.md) **cada onPremisesPublishingProfile** a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes. A [configuração](hybridagentupdaterconfiguration.md) do atualizador especificada para um **onPremisesPublishingProfile** é aplicável a todos os agentes dentro desse **onPremisesPublishingProfile**.

Para um tutorial sobre como configurar o Proxy de Aplicativo, confira Automatizar a configuração do Proxy de Aplicativo usando a [API do Microsoft Graph.](/graph/application-proxy-configure-api)

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



