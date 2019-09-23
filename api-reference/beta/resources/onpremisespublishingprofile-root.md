---
title: Perfis de publicação no local
description: Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 73fbd77064f434b93b3dca91d3bc28d5b4101aba
ms.sourcegitcommit: e87be8765d7f2bc90c6244d84c4719468bb3fd25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2019
ms.locfileid: "37113897"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="56aa5-103">Perfis de publicação no local</span><span class="sxs-lookup"><span data-stu-id="56aa5-103">On-premises publishing profiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56aa5-104">Vários serviços do Azure (por exemplo, autenticação de passagem do Azure Active Directory Connect, WORKDAY para o provisionamento de usuários do Azure AD) permitem um acesso condicional a vários recursos locais de fora da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="56aa5-104">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="56aa5-105">[Os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.</span><span class="sxs-lookup"><span data-stu-id="56aa5-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="56aa5-106">Os [grupos de agentes](onpremisesagentgroup.md) permitem que um administrador de locatários atribua agentes específicos para atender recursos locais publicados específicos.</span><span class="sxs-lookup"><span data-stu-id="56aa5-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="56aa5-107">Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo.</span><span class="sxs-lookup"><span data-stu-id="56aa5-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="56aa5-108">Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="56aa5-108">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="56aa5-109">Um administrador de locatários pode configurar para cada **onPremisesPublishingProfile** a [janela de tempo](updatewindow.md) durante a qual os agentes podem receber atualizações ou adiar atualizações para os agentes.</span><span class="sxs-lookup"><span data-stu-id="56aa5-109">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="56aa5-110">A [configuração de atualizador](hybridagentupdaterconfiguration.md) especificada para um **onPremisesPublishingProfile** é aplicável a todos os agentes dentro desse **onPremisesPublishingProfile**.</span><span class="sxs-lookup"><span data-stu-id="56aa5-110">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

## <a name="see-also"></a><span data-ttu-id="56aa5-111">Confira também</span><span class="sxs-lookup"><span data-stu-id="56aa5-111">See also</span></span>

- [<span data-ttu-id="56aa5-112">Agente local</span><span class="sxs-lookup"><span data-stu-id="56aa5-112">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="56aa5-113">Grupo de agentes local</span><span class="sxs-lookup"><span data-stu-id="56aa5-113">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="56aa5-114">Perfil de publicação local</span><span class="sxs-lookup"><span data-stu-id="56aa5-114">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="56aa5-115">Recurso publicado</span><span class="sxs-lookup"><span data-stu-id="56aa5-115">Published resource</span></span>](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
