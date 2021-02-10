---
title: tipo de recurso room
description: Especifica as propriedades de uma sala em um locatário.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3936338aee39eb0c10a179e5d1970b3e18493214
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156326"
---
# <a name="room-resource-type"></a><span data-ttu-id="aa14c-103">tipo de recurso room</span><span class="sxs-lookup"><span data-stu-id="aa14c-103">room resource type</span></span>

<span data-ttu-id="aa14c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa14c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa14c-105">Representa uma sala em um locatário.</span><span class="sxs-lookup"><span data-stu-id="aa14c-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="aa14c-106">No Exchange Online, cada sala é associada a uma caixa de correio de sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="aa14c-107">Derivado do [local.](place.md)</span><span class="sxs-lookup"><span data-stu-id="aa14c-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aa14c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="aa14c-108">Methods</span></span>

| <span data-ttu-id="aa14c-109">Método</span><span class="sxs-lookup"><span data-stu-id="aa14c-109">Method</span></span>                              | <span data-ttu-id="aa14c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aa14c-110">Return Type</span></span>                  | <span data-ttu-id="aa14c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa14c-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="aa14c-112">Listar locais</span><span class="sxs-lookup"><span data-stu-id="aa14c-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="aa14c-113">Uma coleção do tipo de local [](place.md) solicitado derivado</span><span class="sxs-lookup"><span data-stu-id="aa14c-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="aa14c-114">Obter uma coleção do tipo especificado de objeto **de** local definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="aa14c-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="aa14c-115">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="aa14c-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="aa14c-116">Obter local</span><span class="sxs-lookup"><span data-stu-id="aa14c-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="aa14c-117">O tipo de local [](place.md) solicitado derivado</span><span class="sxs-lookup"><span data-stu-id="aa14c-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="aa14c-118">Obter as propriedades e as relações do objeto **de local** especificado, como uma sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa14c-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa14c-119">Properties</span></span>

| <span data-ttu-id="aa14c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa14c-120">Property</span></span>               | <span data-ttu-id="aa14c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa14c-121">Type</span></span>                                              | <span data-ttu-id="aa14c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa14c-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="aa14c-123">address</span><span class="sxs-lookup"><span data-stu-id="aa14c-123">address</span></span>                | [<span data-ttu-id="aa14c-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="aa14c-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="aa14c-125">O endereço da sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-125">The street address of the room.</span></span> |
| <span data-ttu-id="aa14c-126">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="aa14c-126">audioDeviceName</span></span>        | <span data-ttu-id="aa14c-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-127">String</span></span>                                            | <span data-ttu-id="aa14c-128">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="aa14c-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="aa14c-129">bookingType</span></span>            | [<span data-ttu-id="aa14c-130">bookingType</span><span class="sxs-lookup"><span data-stu-id="aa14c-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="aa14c-131">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-131">Type of room.</span></span> <span data-ttu-id="aa14c-132">Os valores possíveis `standard` são `reserved` e.</span><span class="sxs-lookup"><span data-stu-id="aa14c-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="aa14c-133">building</span><span class="sxs-lookup"><span data-stu-id="aa14c-133">building</span></span>               | <span data-ttu-id="aa14c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-134">String</span></span>                                            | <span data-ttu-id="aa14c-135">Especifica o nome do edifício ou o número do edifício em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="aa14c-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="aa14c-136">capacity</span><span class="sxs-lookup"><span data-stu-id="aa14c-136">capacity</span></span>               | <span data-ttu-id="aa14c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="aa14c-137">Int32</span></span>                                             | <span data-ttu-id="aa14c-138">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="aa14c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="aa14c-139">displayName</span></span>            | <span data-ttu-id="aa14c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-140">String</span></span>                                            | <span data-ttu-id="aa14c-141">O nome associado à sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-141">The name associated with the room.</span></span> |
| <span data-ttu-id="aa14c-142">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="aa14c-142">displayDeviceName</span></span>      | <span data-ttu-id="aa14c-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-143">String</span></span>                                            | <span data-ttu-id="aa14c-144">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="aa14c-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="aa14c-145">emailAddress</span></span>           | <span data-ttu-id="aa14c-146">String</span><span class="sxs-lookup"><span data-stu-id="aa14c-146">String</span></span>                                            | <span data-ttu-id="aa14c-147">Endereço de email da sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-147">Email address of the room.</span></span> |
| <span data-ttu-id="aa14c-148">floorLabel</span><span class="sxs-lookup"><span data-stu-id="aa14c-148">floorLabel</span></span>             | <span data-ttu-id="aa14c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-149">String</span></span>                                            | <span data-ttu-id="aa14c-150">Especifica um rótulo descritivo para o piso, por exemplo, P.</span><span class="sxs-lookup"><span data-stu-id="aa14c-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="aa14c-151">floorNumber</span><span class="sxs-lookup"><span data-stu-id="aa14c-151">floorNumber</span></span>            | <span data-ttu-id="aa14c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="aa14c-152">Int32</span></span>                                             | <span data-ttu-id="aa14c-153">Especifica o número do piso em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="aa14c-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="aa14c-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="aa14c-154">geoCoordinates</span></span>         | [<span data-ttu-id="aa14c-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="aa14c-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="aa14c-156">Especifica o local da sala em coordenadas de latitude, longitude e, opcionalmente, altitude.</span><span class="sxs-lookup"><span data-stu-id="aa14c-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="aa14c-157">id</span><span class="sxs-lookup"><span data-stu-id="aa14c-157">id</span></span>                     | <span data-ttu-id="aa14c-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-158">String</span></span>                                            | <span data-ttu-id="aa14c-159">Identificador exclusivo da sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-159">Unique identifier for the room.</span></span> <span data-ttu-id="aa14c-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa14c-160">Read-only.</span></span> |
| <span data-ttu-id="aa14c-161">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="aa14c-161">isWheelChairAccessible</span></span> | <span data-ttu-id="aa14c-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa14c-162">Boolean</span></span>                                           | <span data-ttu-id="aa14c-163">Especifica se a sala é acessível para acessibilidade.</span><span class="sxs-lookup"><span data-stu-id="aa14c-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="aa14c-164">rótulo</span><span class="sxs-lookup"><span data-stu-id="aa14c-164">label</span></span>                  | <span data-ttu-id="aa14c-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-165">String</span></span>                                            | <span data-ttu-id="aa14c-166">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="aa14c-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="aa14c-167">nickname</span><span class="sxs-lookup"><span data-stu-id="aa14c-167">nickname</span></span>               | <span data-ttu-id="aa14c-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-168">String</span></span>                                            | <span data-ttu-id="aa14c-169">Especifica um apelido para a sala, por exemplo, "conf room".</span><span class="sxs-lookup"><span data-stu-id="aa14c-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="aa14c-170">phone</span><span class="sxs-lookup"><span data-stu-id="aa14c-170">phone</span></span>                  | <span data-ttu-id="aa14c-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-171">String</span></span>                                            | <span data-ttu-id="aa14c-172">O número de telefone da sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-172">The phone number of the room.</span></span> |
| <span data-ttu-id="aa14c-173">tags</span><span class="sxs-lookup"><span data-stu-id="aa14c-173">tags</span></span>                   | <span data-ttu-id="aa14c-174">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-174">String collection</span></span>                                 | <span data-ttu-id="aa14c-175">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou o tipo de móveis.</span><span class="sxs-lookup"><span data-stu-id="aa14c-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="aa14c-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="aa14c-176">videoDeviceName</span></span>        | <span data-ttu-id="aa14c-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa14c-177">String</span></span>                                            | <span data-ttu-id="aa14c-178">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="aa14c-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="aa14c-179">valores de bookingType</span><span class="sxs-lookup"><span data-stu-id="aa14c-179">bookingType values</span></span>

| <span data-ttu-id="aa14c-180">Valor</span><span class="sxs-lookup"><span data-stu-id="aa14c-180">Value</span></span>    | <span data-ttu-id="aa14c-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa14c-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="aa14c-182">padrão</span><span class="sxs-lookup"><span data-stu-id="aa14c-182">standard</span></span> | <span data-ttu-id="aa14c-183">A sala está disponível e pode ser reservada.</span><span class="sxs-lookup"><span data-stu-id="aa14c-183">The room is available and can be reserved.</span></span> <span data-ttu-id="aa14c-184">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="aa14c-184">This is the default value.</span></span> |
| <span data-ttu-id="aa14c-185">reservado</span><span class="sxs-lookup"><span data-stu-id="aa14c-185">reserved</span></span> | <span data-ttu-id="aa14c-186">A sala está disponível somente na primeira vez que for servido pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="aa14c-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="aa14c-187">Ele não pode ser reservado.</span><span class="sxs-lookup"><span data-stu-id="aa14c-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa14c-188">Relações</span><span class="sxs-lookup"><span data-stu-id="aa14c-188">Relationships</span></span>

<span data-ttu-id="aa14c-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa14c-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa14c-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa14c-190">JSON representation</span></span>

<span data-ttu-id="aa14c-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa14c-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": 1024,
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelChairAccessible": true,
  "label": "String",
  "nickname": "String",
  "phone": "String",
  "tags": ["String"],
  "videoDeviceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "room resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

