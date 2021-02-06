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
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="92614-103">Perfis de publicação local</span><span class="sxs-lookup"><span data-stu-id="92614-103">On-premises publishing profiles</span></span>

<span data-ttu-id="92614-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92614-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92614-105">Vários serviços do Azure (por exemplo, a Autenticação de Passagem do Azure Active Directory [Connect,](/azure/active-directory/hybrid/how-to-connect-pta)o dia de trabalho para o provisionamento de usuários do [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [Proxy](https://aka.ms/whyappproxy)  de aplicativo permitem acesso a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="92614-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy)  allow access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="92614-106">[Agentes locais (ou](onpremisesagent.md) conectores para Proxy de Aplicativo) instalados por um administrador de locatários podem ser [configurados](connector.md) para encaminhar solicitações para um recurso [publicado específico.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="92614-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by a tenant administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="92614-107">[Grupos de agentes](onpremisesagentgroup.md) (ou [grupos de](connectorgroup.md) conectores para Proxy de Aplicativo) permitem que um administrador de locatários atribua agentes específicos para atender a recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="92614-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="92614-108">Os administradores de locatários podem agrupar vários agentes e atribuir cada recurso publicado a um grupo.</span><span class="sxs-lookup"><span data-stu-id="92614-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="92614-109">Todo o conjunto de entidades do mesmo tipo de publicação local é representado por [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="92614-109">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="92614-110">Um administrador de locatários pode configurar para [](updatewindow.md) **cada onPremisesPublishingProfile** a janela de tempo durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes.</span><span class="sxs-lookup"><span data-stu-id="92614-110">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="92614-111">A [configuração](hybridagentupdaterconfiguration.md) do atualizador especificada para um **onPremisesPublishingProfile** é aplicável a todos os agentes dentro desse **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="92614-111">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

<span data-ttu-id="92614-112">Para um tutorial sobre como configurar o Proxy de Aplicativo, confira Automatizar a configuração do Proxy de Aplicativo usando a [API do Microsoft Graph.](/graph/application-proxy-configure-api)</span><span class="sxs-lookup"><span data-stu-id="92614-112">For a tutorial about configuring Application Proxy, see [Automate the configuration of Application Proxy using the Microsoft Graph API](/graph/application-proxy-configure-api).</span></span>

## <a name="see-also"></a><span data-ttu-id="92614-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="92614-113">See also</span></span>

- [<span data-ttu-id="92614-114">Agente local</span><span class="sxs-lookup"><span data-stu-id="92614-114">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="92614-115">Grupo de agentes local</span><span class="sxs-lookup"><span data-stu-id="92614-115">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="92614-116">Perfil de publicação local</span><span class="sxs-lookup"><span data-stu-id="92614-116">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="92614-117">Recurso publicado</span><span class="sxs-lookup"><span data-stu-id="92614-117">Published resource</span></span>](publishedresource.md)
- [<span data-ttu-id="92614-118">Connector</span><span class="sxs-lookup"><span data-stu-id="92614-118">Connector</span></span>](connector.md)
- [<span data-ttu-id="92614-119">Grupo de conectores</span><span class="sxs-lookup"><span data-stu-id="92614-119">Connector group</span></span>](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



