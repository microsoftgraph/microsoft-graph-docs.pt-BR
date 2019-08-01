---
title: Tipo de recurso locationConstraintItem
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ee841112aa641069ec64d744120f460713e51c7d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036453"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="48002-103">Tipo de recurso locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="48002-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="48002-104">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="48002-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="48002-105">Derivado de [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="48002-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="48002-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48002-106">JSON representation</span></span>

<span data-ttu-id="48002-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="48002-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="48002-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48002-108">Properties</span></span>
| <span data-ttu-id="48002-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48002-109">Property</span></span>     | <span data-ttu-id="48002-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="48002-110">Type</span></span>   |<span data-ttu-id="48002-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="48002-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48002-112">address</span><span class="sxs-lookup"><span data-stu-id="48002-112">address</span></span> | [<span data-ttu-id="48002-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="48002-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="48002-114">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="48002-114">The street address of the location.</span></span> |
| <span data-ttu-id="48002-115">displayName</span><span class="sxs-lookup"><span data-stu-id="48002-115">displayName</span></span>  | <span data-ttu-id="48002-116">String</span><span class="sxs-lookup"><span data-stu-id="48002-116">String</span></span> | <span data-ttu-id="48002-117">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="48002-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="48002-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="48002-118">locationEmailAddress</span></span> | <span data-ttu-id="48002-119">String</span><span class="sxs-lookup"><span data-stu-id="48002-119">String</span></span> | <span data-ttu-id="48002-120">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="48002-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="48002-121">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="48002-121">resolveAvailability</span></span> | <span data-ttu-id="48002-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="48002-122">Boolean</span></span> | <span data-ttu-id="48002-p101">Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user-findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="48002-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
