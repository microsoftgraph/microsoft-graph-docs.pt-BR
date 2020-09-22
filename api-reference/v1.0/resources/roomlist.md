---
title: tipo de recurso RoomList
description: Representa um grupo de salas criadas pela empresa.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d4563ef9fec149c219fe6eae25a4ba3344fbd90d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088479"
---
# <a name="roomlist-resource-type"></a><span data-ttu-id="33349-103">tipo de recurso RoomList</span><span class="sxs-lookup"><span data-stu-id="33349-103">roomList resource type</span></span>

<span data-ttu-id="33349-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33349-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33349-105">Representa um grupo de objetos [Room](room.md) definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="33349-105">Represents a group of [room](room.md) objects defined in the tenant.</span></span>

<span data-ttu-id="33349-106">Derivado do [local](place.md).</span><span class="sxs-lookup"><span data-stu-id="33349-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="33349-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="33349-107">Methods</span></span>

| <span data-ttu-id="33349-108">Método</span><span class="sxs-lookup"><span data-stu-id="33349-108">Method</span></span>                              | <span data-ttu-id="33349-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="33349-109">Return Type</span></span>                  | <span data-ttu-id="33349-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="33349-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="33349-111">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="33349-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="33349-112">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="33349-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="33349-113">Obtém uma coleção do tipo especificado do objeto **Place** definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="33349-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="33349-114">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="33349-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>|
| [<span data-ttu-id="33349-115">Obter local</span><span class="sxs-lookup"><span data-stu-id="33349-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="33349-116">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="33349-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="33349-117">Obtenha as propriedades e os relacionamentos do objeto **local** especificado, como uma lista de salas.</span><span class="sxs-lookup"><span data-stu-id="33349-117">Get the properties and relationships of the specified **place** object, such as a room list.</span></span> |

## <a name="properties"></a><span data-ttu-id="33349-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33349-118">Properties</span></span>

| <span data-ttu-id="33349-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33349-119">Property</span></span>       | <span data-ttu-id="33349-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="33349-120">Type</span></span>                                              | <span data-ttu-id="33349-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="33349-121">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="33349-122">address</span><span class="sxs-lookup"><span data-stu-id="33349-122">address</span></span>        | [<span data-ttu-id="33349-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="33349-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="33349-124">O endereço da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="33349-124">The street address of the room list.</span></span> |
| <span data-ttu-id="33349-125">displayName</span><span class="sxs-lookup"><span data-stu-id="33349-125">displayName</span></span>    | <span data-ttu-id="33349-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33349-126">String</span></span>                                            | <span data-ttu-id="33349-127">O nome associado à lista de salas.</span><span class="sxs-lookup"><span data-stu-id="33349-127">The name associated with the room list.</span></span> |
| <span data-ttu-id="33349-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="33349-128">emailAddress</span></span>   | <span data-ttu-id="33349-129">String</span><span class="sxs-lookup"><span data-stu-id="33349-129">String</span></span>                                            | <span data-ttu-id="33349-130">O endereço de email da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="33349-130">The email address of the room list.</span></span> |
| <span data-ttu-id="33349-131">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="33349-131">geoCoordinates</span></span> | [<span data-ttu-id="33349-132">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="33349-132">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="33349-133">Especifica o local da sala de opções no latitude, longitude e (opcionalmente) as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="33349-133">Specifies the roomlist location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="33349-134">id</span><span class="sxs-lookup"><span data-stu-id="33349-134">id</span></span>             | <span data-ttu-id="33349-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33349-135">String</span></span>                                            | <span data-ttu-id="33349-136">Identificador exclusivo da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="33349-136">Unique identifier for the room list.</span></span> <span data-ttu-id="33349-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="33349-137">Read-only.</span></span> |
| <span data-ttu-id="33349-138">phone</span><span class="sxs-lookup"><span data-stu-id="33349-138">phone</span></span>          | <span data-ttu-id="33349-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33349-139">String</span></span>                                            | <span data-ttu-id="33349-140">O número de telefone da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="33349-140">The phone number of the room list.</span></span> |

## <a name="relationships"></a><span data-ttu-id="33349-141">Relações</span><span class="sxs-lookup"><span data-stu-id="33349-141">Relationships</span></span>

| <span data-ttu-id="33349-142">Relação</span><span class="sxs-lookup"><span data-stu-id="33349-142">Relationship</span></span> | <span data-ttu-id="33349-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="33349-143">Type</span></span>                         | <span data-ttu-id="33349-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="33349-144">Description</span></span>          |
|:-------------|:-----------------------------|:---------------------|
| <span data-ttu-id="33349-145">quartos</span><span class="sxs-lookup"><span data-stu-id="33349-145">rooms</span></span>        | <span data-ttu-id="33349-146">[colocar](place.md) coleção</span><span class="sxs-lookup"><span data-stu-id="33349-146">[place](place.md) collection</span></span> | <span data-ttu-id="33349-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="33349-p103">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="33349-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33349-149">JSON representation</span></span>

<span data-ttu-id="33349-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33349-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roomList"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "emailAddress": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "phone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roomList resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

