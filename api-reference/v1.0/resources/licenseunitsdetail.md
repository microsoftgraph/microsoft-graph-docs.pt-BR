---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
author: 'michaelcurnutt '
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 523a8c65d7588a1626d085efde1beea99bdf9643
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030940"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="06e0a-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="06e0a-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="06e0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06e0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06e0a-105">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="06e0a-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span> <span data-ttu-id="06e0a-106">Para obter mais informações sobre os estados de progressão de uma assinatura, consulte [E se minha assinatura expirar?](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="06e0a-106">For more information on the progression states of a subscription, see [What if my subscription expires?](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)</span></span>

## <a name="properties"></a><span data-ttu-id="06e0a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06e0a-107">Properties</span></span>
| <span data-ttu-id="06e0a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06e0a-108">Property</span></span>     | <span data-ttu-id="06e0a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="06e0a-109">Type</span></span>   |<span data-ttu-id="06e0a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06e0a-110">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="06e0a-111">enabled</span><span class="sxs-lookup"><span data-stu-id="06e0a-111">enabled</span></span>|<span data-ttu-id="06e0a-112">Int32</span><span class="sxs-lookup"><span data-stu-id="06e0a-112">Int32</span></span>| <span data-ttu-id="06e0a-113">O número de unidades habilitadas para a assinatura ativa do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="06e0a-113">The number of units that are enabled for the active subscription of the service SKU.</span></span>  |
|<span data-ttu-id="06e0a-114">suspended</span><span class="sxs-lookup"><span data-stu-id="06e0a-114">suspended</span></span>|<span data-ttu-id="06e0a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="06e0a-115">Int32</span></span>| <span data-ttu-id="06e0a-116">O número de unidades suspensas porque a assinatura do SKU do serviço foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="06e0a-116">The number of units that are suspended because the subscription of the service SKU has been cancelled.</span></span> <span data-ttu-id="06e0a-117">As unidades não podem ser atribuídas, mas ainda podem ser reativadas antes de serem excluídas.</span><span class="sxs-lookup"><span data-stu-id="06e0a-117">The units cannot be assigned but can still be reactivated before they are deleted.</span></span> |
|<span data-ttu-id="06e0a-118">warning</span><span class="sxs-lookup"><span data-stu-id="06e0a-118">warning</span></span>|<span data-ttu-id="06e0a-119">Int32</span><span class="sxs-lookup"><span data-stu-id="06e0a-119">Int32</span></span>| <span data-ttu-id="06e0a-120">O número de unidades que estão em status de aviso.</span><span class="sxs-lookup"><span data-stu-id="06e0a-120">The number of units that are in warning status.</span></span> <span data-ttu-id="06e0a-121">Quando a assinatura do SKU do serviço expirou, o cliente tem um período de carência para renovar sua assinatura antes de ser cancelada (movida para um **estado suspenso).**</span><span class="sxs-lookup"><span data-stu-id="06e0a-121">When the subscription of the service SKU has expired, the customer has a grace period to renew their subscription before it is cancelled (moved to a **suspended** state).</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="06e0a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06e0a-122">JSON representation</span></span>

<span data-ttu-id="06e0a-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="06e0a-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

