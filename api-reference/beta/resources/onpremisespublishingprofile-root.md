---
title: Perfis de publicação local
description: Vários serviços do Azure (por exemplo, Azure Active Directory Conexão autenticação passo a passo, o provisionamento de usuários do Workday para o Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: b8bb4a485f06ea45d553134668fff241984b2ad8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095520"
---
# <a name="on-premises-publishing-profiles"></a>Perfis de publicação local

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Vários serviços do Azure (por exemplo, Azure Active Directory Conexão autenticação passo [a](/azure/active-directory/hybrid/how-to-connect-pta)passo, dia de trabalho para o provisionamento de usuários do [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)e [Proxy](/azure/active-directory/app-proxy/what-is-application-proxy) de Aplicativo permitem acesso a vários recursos locais de fora da rede corporativa. Agentes locais (ou conectores para Proxy de Aplicativo) [instalados](connector.md) por um administrador de locatários podem ser [configurados](onpremisesagent.md) para rotear solicitações para um determinado [recurso publicado.](publishedresource.md)
[Grupos de agentes](onpremisesagentgroup.md) (ou [grupos de](connectorgroup.md) conectores para Proxy de Aplicativo) permitem que um administrador de locatário atribua agentes específicos para atender a recursos locais publicados específicos. Os administradores de locatários podem agrupar vários agentes e atribuir cada recurso publicado a um grupo. Todo o conjunto de entidades do mesmo tipo de publicação local é representado por [onPremisesPublishingProfile](onpremisespublishingprofile.md).

Um administrador de locatário pode configurar para cada [](updatewindow.md) **onPremisesPublishingProfile** a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes. A [configuração do](hybridagentupdaterconfiguration.md) atualizador especificada para **um onPremisesPublishingProfile** é aplicável a todos os agentes dentro desse **onPremisesPublishingProfile**.

Para um tutorial sobre como configurar o Proxy de Aplicativo, consulte [Automate the configuration of Application Proxy using the Microsoft Graph API](/graph/application-proxy-configure-api).

## <a name="see-also"></a>Confira também

- [Agente local](onpremisesagent.md)
- [Grupo de agentes locais](onpremisesagentgroup.md)
- [Perfil de publicação local](onpremisespublishingprofile.md)
- [Recurso publicado](publishedresource.md)
- [Connector](connector.md)
- [Grupo Conector](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->