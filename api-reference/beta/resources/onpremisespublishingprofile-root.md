---
title: Perfis de publicação no local
description: Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1e2403d057cc399279ec8ac3084e67798092705b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998641"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="17adf-103">Perfis de publicação no local</span><span class="sxs-lookup"><span data-stu-id="17adf-103">On-premises publishing profiles</span></span>

<span data-ttu-id="17adf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17adf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17adf-105">Vários serviços do Azure (por exemplo, a autenticação de [passagem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)do Azure Active Directory Connect, o [WORKDAY para o provisionamento de usuários do Azure ad](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [proxy de aplicativo](https://aka.ms/whyappproxy)  permitem o acesso a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="17adf-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy)  allow access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="17adf-106">[Os agentes locais](onpremisesagent.md) (ou [conectores](connector.md) para o proxy de aplicativo) instalados por um administrador de locatários podem ser configurados para rotear solicitações para um determinado [recurso publicado](publishedresource.md).</span><span class="sxs-lookup"><span data-stu-id="17adf-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by a tenant administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="17adf-107">Os [grupos de agentes](onpremisesagentgroup.md) (ou grupos de [conectores](connectorgroup.md) para o proxy de aplicativo) permitem que um administrador de locatários atribua agentes específicos para atender a recursos específicos publicados no local.</span><span class="sxs-lookup"><span data-stu-id="17adf-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="17adf-108">Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo.</span><span class="sxs-lookup"><span data-stu-id="17adf-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="17adf-109">Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="17adf-109">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="17adf-110">Um administrador de locatários pode configurar para cada **onPremisesPublishingProfile** a [janela de tempo](updatewindow.md) durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes.</span><span class="sxs-lookup"><span data-stu-id="17adf-110">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="17adf-111">A [configuração de atualizador](hybridagentupdaterconfiguration.md) especificada para um **onPremisesPublishingProfile** é aplicável a todos os agentes dentro desse **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="17adf-111">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

<span data-ttu-id="17adf-112">Para obter um tutorial sobre a configuração do proxy de aplicativo, consulte [automatizar a configuração do proxy de aplicativo usando a API do Microsoft Graph](https://docs.microsoft.com/graph/application-proxy-configure-api).</span><span class="sxs-lookup"><span data-stu-id="17adf-112">For a tutorial about configuring Application Proxy, see [Automate the configuration of Application Proxy using the Microsoft Graph API](https://docs.microsoft.com/graph/application-proxy-configure-api).</span></span>

## <a name="see-also"></a><span data-ttu-id="17adf-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="17adf-113">See also</span></span>

- [<span data-ttu-id="17adf-114">Agente local</span><span class="sxs-lookup"><span data-stu-id="17adf-114">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="17adf-115">Grupo de agentes local</span><span class="sxs-lookup"><span data-stu-id="17adf-115">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="17adf-116">Perfil de publicação local</span><span class="sxs-lookup"><span data-stu-id="17adf-116">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="17adf-117">Recurso publicado</span><span class="sxs-lookup"><span data-stu-id="17adf-117">Published resource</span></span>](publishedresource.md)
- [<span data-ttu-id="17adf-118">Connector</span><span class="sxs-lookup"><span data-stu-id="17adf-118">Connector</span></span>](connector.md)
- [<span data-ttu-id="17adf-119">Grupo de conectores</span><span class="sxs-lookup"><span data-stu-id="17adf-119">Connector group</span></span>](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


