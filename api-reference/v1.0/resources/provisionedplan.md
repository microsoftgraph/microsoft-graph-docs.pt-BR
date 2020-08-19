---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8b7f3e5ac0c66dca2cb297986af1be6473de23c1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806874"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="5b618-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="5b618-103">provisionedPlan resource type</span></span>

<span data-ttu-id="5b618-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b618-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b618-105">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="5b618-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="5b618-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b618-106">Properties</span></span>
| <span data-ttu-id="5b618-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b618-107">Property</span></span>     | <span data-ttu-id="5b618-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b618-108">Type</span></span>   |<span data-ttu-id="5b618-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b618-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b618-110">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="5b618-110">capabilityStatus</span></span>|<span data-ttu-id="5b618-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b618-111">String</span></span>|<span data-ttu-id="5b618-112">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="5b618-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="5b618-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="5b618-113">provisioningStatus</span></span>|<span data-ttu-id="5b618-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b618-114">String</span></span>|<span data-ttu-id="5b618-115">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="5b618-115">For example, “Success”.</span></span>|
|<span data-ttu-id="5b618-116">service</span><span class="sxs-lookup"><span data-stu-id="5b618-116">service</span></span>|<span data-ttu-id="5b618-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b618-117">String</span></span>|<span data-ttu-id="5b618-118">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="5b618-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b618-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b618-119">JSON representation</span></span>

<span data-ttu-id="5b618-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5b618-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
