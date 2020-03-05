---
title: tipo de recurso RoomList
description: Representa um grupo de salas criadas pela empresa.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3aa89075b93f34ad565d210bee3dff2bfd1ffe81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521030"
---
# <a name="roomlist-resource-type"></a><span data-ttu-id="4242b-103">tipo de recurso RoomList</span><span class="sxs-lookup"><span data-stu-id="4242b-103">roomList resource type</span></span>

<span data-ttu-id="4242b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4242b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4242b-105">Representa um grupo de objetos [Room](room.md) definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="4242b-105">Represents a group of [room](room.md) objects defined in the tenant.</span></span>

<span data-ttu-id="4242b-106">Derivado do [local](place.md).</span><span class="sxs-lookup"><span data-stu-id="4242b-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4242b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4242b-107">Methods</span></span>

| <span data-ttu-id="4242b-108">Método</span><span class="sxs-lookup"><span data-stu-id="4242b-108">Method</span></span>                              | <span data-ttu-id="4242b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4242b-109">Return Type</span></span>                  | <span data-ttu-id="4242b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4242b-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="4242b-111">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="4242b-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="4242b-112">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="4242b-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="4242b-113">Obtém uma coleção do tipo especificado do objeto **Place** definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="4242b-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="4242b-114">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="4242b-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>|
| [<span data-ttu-id="4242b-115">Obter local</span><span class="sxs-lookup"><span data-stu-id="4242b-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="4242b-116">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="4242b-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="4242b-117">Obtenha as propriedades e os relacionamentos do objeto **local** especificado, como uma lista de salas.</span><span class="sxs-lookup"><span data-stu-id="4242b-117">Get the properties and relationships of the specified **place** object, such as a room list.</span></span> |

## <a name="properties"></a><span data-ttu-id="4242b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4242b-118">Properties</span></span>

| <span data-ttu-id="4242b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4242b-119">Property</span></span>       | <span data-ttu-id="4242b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4242b-120">Type</span></span>                                              | <span data-ttu-id="4242b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4242b-121">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="4242b-122">address</span><span class="sxs-lookup"><span data-stu-id="4242b-122">address</span></span>        | [<span data-ttu-id="4242b-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4242b-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="4242b-124">O endereço da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="4242b-124">The street address of the room list.</span></span> |
| <span data-ttu-id="4242b-125">displayName</span><span class="sxs-lookup"><span data-stu-id="4242b-125">displayName</span></span>    | <span data-ttu-id="4242b-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4242b-126">String</span></span>                                            | <span data-ttu-id="4242b-127">O nome associado à lista de salas.</span><span class="sxs-lookup"><span data-stu-id="4242b-127">The name associated with the room list.</span></span> |
| <span data-ttu-id="4242b-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4242b-128">emailAddress</span></span>   | <span data-ttu-id="4242b-129">String</span><span class="sxs-lookup"><span data-stu-id="4242b-129">String</span></span>                                            | <span data-ttu-id="4242b-130">O endereço de email da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="4242b-130">The email address of the room list.</span></span> |
| <span data-ttu-id="4242b-131">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="4242b-131">geoCoordinates</span></span> | [<span data-ttu-id="4242b-132">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="4242b-132">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="4242b-133">Especifica o local da sala de opções no latitude, longitude e (opcionalmente) as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="4242b-133">Specifies the roomlist location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="4242b-134">id</span><span class="sxs-lookup"><span data-stu-id="4242b-134">id</span></span>             | <span data-ttu-id="4242b-135">String</span><span class="sxs-lookup"><span data-stu-id="4242b-135">String</span></span>                                            | <span data-ttu-id="4242b-136">Identificador exclusivo da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="4242b-136">Unique identifier for the room list.</span></span> <span data-ttu-id="4242b-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4242b-137">Read-only.</span></span> |
| <span data-ttu-id="4242b-138">phone</span><span class="sxs-lookup"><span data-stu-id="4242b-138">phone</span></span>          | <span data-ttu-id="4242b-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4242b-139">String</span></span>                                            | <span data-ttu-id="4242b-140">O número de telefone da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="4242b-140">The phone number of the room list.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4242b-141">Relações</span><span class="sxs-lookup"><span data-stu-id="4242b-141">Relationships</span></span>

| <span data-ttu-id="4242b-142">Relação</span><span class="sxs-lookup"><span data-stu-id="4242b-142">Relationship</span></span> | <span data-ttu-id="4242b-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="4242b-143">Type</span></span>                         | <span data-ttu-id="4242b-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="4242b-144">Description</span></span>          |
|:-------------|:-----------------------------|:---------------------|
| <span data-ttu-id="4242b-145">quartos</span><span class="sxs-lookup"><span data-stu-id="4242b-145">rooms</span></span>        | <span data-ttu-id="4242b-146">[colocar](place.md) coleção</span><span class="sxs-lookup"><span data-stu-id="4242b-146">[place](place.md) collection</span></span> | <span data-ttu-id="4242b-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="4242b-p103">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4242b-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4242b-149">JSON representation</span></span>

<span data-ttu-id="4242b-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4242b-150">The following is a JSON representation of the resource.</span></span>

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
