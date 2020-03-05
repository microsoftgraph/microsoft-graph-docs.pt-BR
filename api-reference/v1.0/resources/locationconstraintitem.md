---
title: Tipo de recurso locationConstraintItem
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 404b0fd380c1161a827fe4610f744d0b9872c92b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447525"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="436a8-103">Tipo de recurso locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="436a8-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="436a8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="436a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="436a8-105">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="436a8-105">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="436a8-106">Derivado de [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="436a8-106">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="436a8-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="436a8-107">JSON representation</span></span>

<span data-ttu-id="436a8-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="436a8-108">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="436a8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="436a8-109">Properties</span></span>
| <span data-ttu-id="436a8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="436a8-110">Property</span></span>     | <span data-ttu-id="436a8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="436a8-111">Type</span></span>   |<span data-ttu-id="436a8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="436a8-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="436a8-113">address</span><span class="sxs-lookup"><span data-stu-id="436a8-113">address</span></span> | [<span data-ttu-id="436a8-114">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="436a8-114">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="436a8-115">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="436a8-115">The street address of the location.</span></span> |
| <span data-ttu-id="436a8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="436a8-116">displayName</span></span>  | <span data-ttu-id="436a8-117">String</span><span class="sxs-lookup"><span data-stu-id="436a8-117">String</span></span> | <span data-ttu-id="436a8-118">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="436a8-118">The name associated with the location.</span></span>                       |
| <span data-ttu-id="436a8-119">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="436a8-119">locationEmailAddress</span></span> | <span data-ttu-id="436a8-120">String</span><span class="sxs-lookup"><span data-stu-id="436a8-120">String</span></span> | <span data-ttu-id="436a8-121">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="436a8-121">Optional email address of the location.</span></span> |
| <span data-ttu-id="436a8-122">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="436a8-122">resolveAvailability</span></span> | <span data-ttu-id="436a8-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="436a8-123">Boolean</span></span> | <span data-ttu-id="436a8-p101">Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user-findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="436a8-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
