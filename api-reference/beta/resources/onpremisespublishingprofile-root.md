---
title: Perfis de publicação no local
description: Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ae3b31de8a8d4121c836126c09921ef7574301ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522204"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="aed95-103">Perfis de publicação no local</span><span class="sxs-lookup"><span data-stu-id="aed95-103">On-premises publishing profiles</span></span>

<span data-ttu-id="aed95-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aed95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aed95-105">Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="aed95-105">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="aed95-106">[Os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="aed95-106">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="aed95-107">Os [grupos de agentes](onpremisesagentgroup.md) permitem que um administrador de locatários atribua agentes específicos para atender recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="aed95-107">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="aed95-108">Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo.</span><span class="sxs-lookup"><span data-stu-id="aed95-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="aed95-109">Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="aed95-109">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="aed95-110">Um administrador de locatários pode configurar para cada **onPremisesPublishingProfile** a [janela de tempo](updatewindow.md) durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes.</span><span class="sxs-lookup"><span data-stu-id="aed95-110">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="aed95-111">A [configuração de atualizador](hybridagentupdaterconfiguration.md) especificada para um **onPremisesPublishingProfile** é aplicável a todos os agentes dentro desse **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="aed95-111">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

## <a name="see-also"></a><span data-ttu-id="aed95-112">Confira também</span><span class="sxs-lookup"><span data-stu-id="aed95-112">See also</span></span>

- [<span data-ttu-id="aed95-113">Agente local</span><span class="sxs-lookup"><span data-stu-id="aed95-113">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="aed95-114">Grupo de agentes local</span><span class="sxs-lookup"><span data-stu-id="aed95-114">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="aed95-115">Perfil de publicação local</span><span class="sxs-lookup"><span data-stu-id="aed95-115">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="aed95-116">Recurso publicado</span><span class="sxs-lookup"><span data-stu-id="aed95-116">Published resource</span></span>](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
