---
title: tipo de recurso RoomList
description: Representa um grupo de salas criadas pela empresa.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f0c56f986663c71d8c6817c0024919e8714af94a
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841252"
---
# <a name="roomlist-resource-type"></a><span data-ttu-id="b5bfc-103">tipo de recurso RoomList</span><span class="sxs-lookup"><span data-stu-id="b5bfc-103">roomList resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5bfc-104">Representa um grupo de objetos [Room](room.md) definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-104">Represents a group of [room](room.md) objects defined in the tenant.</span></span>

<span data-ttu-id="b5bfc-105">Derivado do [local](place.md).</span><span class="sxs-lookup"><span data-stu-id="b5bfc-105">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b5bfc-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b5bfc-106">Methods</span></span>

| <span data-ttu-id="b5bfc-107">Método</span><span class="sxs-lookup"><span data-stu-id="b5bfc-107">Method</span></span>                              | <span data-ttu-id="b5bfc-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b5bfc-108">Return Type</span></span>                  | <span data-ttu-id="b5bfc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5bfc-109">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="b5bfc-110">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="b5bfc-110">List places</span></span>](../api/place-list.md) | <span data-ttu-id="b5bfc-111">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="b5bfc-111">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="b5bfc-112">Obtém uma coleção do tipo especificado do objeto **Place** definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-112">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="b5bfc-113">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-113">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>|
| [<span data-ttu-id="b5bfc-114">Obter local</span><span class="sxs-lookup"><span data-stu-id="b5bfc-114">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="b5bfc-115">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="b5bfc-115">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="b5bfc-116">Obtenha as propriedades e os relacionamentos do objeto **local** especificado, como uma lista de salas.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-116">Get the properties and relationships of the specified **place** object, such as a room list.</span></span> |

## <a name="properties"></a><span data-ttu-id="b5bfc-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5bfc-117">Properties</span></span>

| <span data-ttu-id="b5bfc-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5bfc-118">Property</span></span>       | <span data-ttu-id="b5bfc-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5bfc-119">Type</span></span>                                              | <span data-ttu-id="b5bfc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5bfc-120">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="b5bfc-121">address</span><span class="sxs-lookup"><span data-stu-id="b5bfc-121">address</span></span>        | [<span data-ttu-id="b5bfc-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b5bfc-122">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="b5bfc-123">O endereço da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-123">The street address of the room list.</span></span> |
| <span data-ttu-id="b5bfc-124">displayName</span><span class="sxs-lookup"><span data-stu-id="b5bfc-124">displayName</span></span>    | <span data-ttu-id="b5bfc-125">String</span><span class="sxs-lookup"><span data-stu-id="b5bfc-125">String</span></span>                                            | <span data-ttu-id="b5bfc-126">O nome associado à lista de salas.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-126">The name associated with the room list.</span></span> |
| <span data-ttu-id="b5bfc-127">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b5bfc-127">emailAddress</span></span>   | <span data-ttu-id="b5bfc-128">String</span><span class="sxs-lookup"><span data-stu-id="b5bfc-128">String</span></span>                                            | <span data-ttu-id="b5bfc-129">O endereço de email da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-129">The email address of the room list.</span></span> |
| <span data-ttu-id="b5bfc-130">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b5bfc-130">geoCoordinates</span></span> | [<span data-ttu-id="b5bfc-131">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b5bfc-131">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="b5bfc-132">Especifica o local da sala de opções no latitude, longitude e (opcionalmente) as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-132">Specifies the roomlist location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="b5bfc-133">id</span><span class="sxs-lookup"><span data-stu-id="b5bfc-133">id</span></span>             | <span data-ttu-id="b5bfc-134">String</span><span class="sxs-lookup"><span data-stu-id="b5bfc-134">String</span></span>                                            | <span data-ttu-id="b5bfc-135">Identificador exclusivo da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-135">Unique identifier for the room list.</span></span> <span data-ttu-id="b5bfc-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-136">Read-only.</span></span> |
| <span data-ttu-id="b5bfc-137">phone</span><span class="sxs-lookup"><span data-stu-id="b5bfc-137">phone</span></span>          | <span data-ttu-id="b5bfc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5bfc-138">String</span></span>                                            | <span data-ttu-id="b5bfc-139">O número de telefone da lista de salas.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-139">The phone number of the room list.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b5bfc-140">Relações</span><span class="sxs-lookup"><span data-stu-id="b5bfc-140">Relationships</span></span>

| <span data-ttu-id="b5bfc-141">Relação</span><span class="sxs-lookup"><span data-stu-id="b5bfc-141">Relationship</span></span> | <span data-ttu-id="b5bfc-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5bfc-142">Type</span></span>                         | <span data-ttu-id="b5bfc-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5bfc-143">Description</span></span>          |
|:-------------|:-----------------------------|:---------------------|
| <span data-ttu-id="b5bfc-144">quartos</span><span class="sxs-lookup"><span data-stu-id="b5bfc-144">rooms</span></span>        | <span data-ttu-id="b5bfc-145">[colocar](place.md) coleção</span><span class="sxs-lookup"><span data-stu-id="b5bfc-145">[place](place.md) collection</span></span> | <span data-ttu-id="b5bfc-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-p103">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b5bfc-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5bfc-148">JSON representation</span></span>

<span data-ttu-id="b5bfc-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5bfc-149">The following is a JSON representation of the resource.</span></span>

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
