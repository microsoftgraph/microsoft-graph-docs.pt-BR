---
title: Tipo de recurso locationConstraintItem
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
ms.openlocfilehash: 4c44a97a3ed0d5bcf56204fab1527c7e4b58455d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874078"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="2865f-103">Tipo de recurso locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="2865f-103">locationConstraintItem resource type</span></span>

> <span data-ttu-id="2865f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2865f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2865f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2865f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2865f-106">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="2865f-106">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="2865f-107">Derivado de [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="2865f-107">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2865f-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2865f-108">JSON representation</span></span>

<span data-ttu-id="2865f-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2865f-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2865f-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2865f-110">Properties</span></span>
| <span data-ttu-id="2865f-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2865f-111">Property</span></span>     | <span data-ttu-id="2865f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="2865f-112">Type</span></span>   |<span data-ttu-id="2865f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2865f-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2865f-114">address</span><span class="sxs-lookup"><span data-stu-id="2865f-114">address</span></span> | [<span data-ttu-id="2865f-115">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2865f-115">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="2865f-116">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="2865f-116">The street address of the location.</span></span> |
| <span data-ttu-id="2865f-117">coordenadas</span><span class="sxs-lookup"><span data-stu-id="2865f-117">coordinates</span></span> | [<span data-ttu-id="2865f-118">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2865f-118">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="2865f-119">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="2865f-119">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="2865f-120">displayName</span><span class="sxs-lookup"><span data-stu-id="2865f-120">displayName</span></span>  | <span data-ttu-id="2865f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2865f-121">String</span></span> | <span data-ttu-id="2865f-122">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="2865f-122">The name associated with the location.</span></span>                       |
| <span data-ttu-id="2865f-123">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2865f-123">locationEmailAddress</span></span> | <span data-ttu-id="2865f-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2865f-124">String</span></span> | <span data-ttu-id="2865f-125">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="2865f-125">Optional email address of the location.</span></span> |
| <span data-ttu-id="2865f-126">locationUri</span><span class="sxs-lookup"><span data-stu-id="2865f-126">locationUri</span></span> | <span data-ttu-id="2865f-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2865f-127">String</span></span> | <span data-ttu-id="2865f-128">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="2865f-128">Optional URI representing the location.</span></span> |
| <span data-ttu-id="2865f-129">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="2865f-129">resolveAvailability</span></span> | <span data-ttu-id="2865f-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="2865f-130">Boolean</span></span> | <span data-ttu-id="2865f-p102">Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user-findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="2865f-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
