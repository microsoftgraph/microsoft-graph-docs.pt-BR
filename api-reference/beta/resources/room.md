---
title: tipo de recurso room
description: Especifica as propriedades de uma sala em um locatário.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1599d029987be2cac8ac33b007dab485bc1474a4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154247"
---
# <a name="room-resource-type"></a><span data-ttu-id="b0ace-103">tipo de recurso room</span><span class="sxs-lookup"><span data-stu-id="b0ace-103">room resource type</span></span>

<span data-ttu-id="b0ace-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0ace-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ace-105">Representa uma sala em um locatário.</span><span class="sxs-lookup"><span data-stu-id="b0ace-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="b0ace-106">No Exchange Online, cada sala é associada a uma caixa de correio de sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="b0ace-107">Derivado do [local.](place.md)</span><span class="sxs-lookup"><span data-stu-id="b0ace-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b0ace-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0ace-108">Methods</span></span>

| <span data-ttu-id="b0ace-109">Método</span><span class="sxs-lookup"><span data-stu-id="b0ace-109">Method</span></span>                              | <span data-ttu-id="b0ace-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0ace-110">Return Type</span></span>                  | <span data-ttu-id="b0ace-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ace-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="b0ace-112">Listar locais</span><span class="sxs-lookup"><span data-stu-id="b0ace-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="b0ace-113">Uma coleção do tipo de local [](place.md) solicitado derivado</span><span class="sxs-lookup"><span data-stu-id="b0ace-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="b0ace-114">Obter uma coleção do tipo especificado de objeto **de** local definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="b0ace-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="b0ace-115">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="b0ace-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="b0ace-116">Obter local</span><span class="sxs-lookup"><span data-stu-id="b0ace-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="b0ace-117">O tipo de local [](place.md) solicitado derivado</span><span class="sxs-lookup"><span data-stu-id="b0ace-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="b0ace-118">Obter as propriedades e as relações do objeto **de local** especificado, como uma sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0ace-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0ace-119">Properties</span></span>

| <span data-ttu-id="b0ace-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0ace-120">Property</span></span>               | <span data-ttu-id="b0ace-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0ace-121">Type</span></span>                                              | <span data-ttu-id="b0ace-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ace-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="b0ace-123">address</span><span class="sxs-lookup"><span data-stu-id="b0ace-123">address</span></span>                | [<span data-ttu-id="b0ace-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b0ace-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="b0ace-125">O endereço da sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-125">The street address of the room.</span></span> |
| <span data-ttu-id="b0ace-126">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="b0ace-126">audioDeviceName</span></span>        | <span data-ttu-id="b0ace-127">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-127">String</span></span>                                            | <span data-ttu-id="b0ace-128">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="b0ace-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="b0ace-129">bookingType</span></span>            | [<span data-ttu-id="b0ace-130">bookingType</span><span class="sxs-lookup"><span data-stu-id="b0ace-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="b0ace-131">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-131">Type of room.</span></span> <span data-ttu-id="b0ace-132">Os valores possíveis `standard` são `reserved` e.</span><span class="sxs-lookup"><span data-stu-id="b0ace-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="b0ace-133">building</span><span class="sxs-lookup"><span data-stu-id="b0ace-133">building</span></span>               | <span data-ttu-id="b0ace-134">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-134">String</span></span>                                            | <span data-ttu-id="b0ace-135">Especifica o nome do edifício ou o número do edifício em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="b0ace-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="b0ace-136">capacity</span><span class="sxs-lookup"><span data-stu-id="b0ace-136">capacity</span></span>               | <span data-ttu-id="b0ace-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ace-137">Int32</span></span>                                             | <span data-ttu-id="b0ace-138">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="b0ace-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b0ace-139">displayName</span></span>            | <span data-ttu-id="b0ace-140">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-140">String</span></span>                                            | <span data-ttu-id="b0ace-141">O nome associado à sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-141">The name associated with the room.</span></span> |
| <span data-ttu-id="b0ace-142">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="b0ace-142">displayDeviceName</span></span>      | <span data-ttu-id="b0ace-143">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-143">String</span></span>                                            | <span data-ttu-id="b0ace-144">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="b0ace-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b0ace-145">emailAddress</span></span>           | <span data-ttu-id="b0ace-146">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-146">String</span></span>                                            | <span data-ttu-id="b0ace-147">Endereço de email da sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-147">Email address of the room.</span></span> |
| <span data-ttu-id="b0ace-148">floorLabel</span><span class="sxs-lookup"><span data-stu-id="b0ace-148">floorLabel</span></span>             | <span data-ttu-id="b0ace-149">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-149">String</span></span>                                            | <span data-ttu-id="b0ace-150">Especifica um rótulo descritivo para o piso, por exemplo, P.</span><span class="sxs-lookup"><span data-stu-id="b0ace-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="b0ace-151">floorNumber</span><span class="sxs-lookup"><span data-stu-id="b0ace-151">floorNumber</span></span>            | <span data-ttu-id="b0ace-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ace-152">Int32</span></span>                                             | <span data-ttu-id="b0ace-153">Especifica o número do piso em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="b0ace-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="b0ace-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b0ace-154">geoCoordinates</span></span>         | [<span data-ttu-id="b0ace-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b0ace-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="b0ace-156">Especifica o local da sala em coordenadas de latitude, longitude e, opcionalmente, altitude.</span><span class="sxs-lookup"><span data-stu-id="b0ace-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="b0ace-157">id</span><span class="sxs-lookup"><span data-stu-id="b0ace-157">id</span></span>                     | <span data-ttu-id="b0ace-158">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-158">String</span></span>                                            | <span data-ttu-id="b0ace-159">Identificador exclusivo da sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-159">Unique identifier for the room.</span></span> <span data-ttu-id="b0ace-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0ace-160">Read-only.</span></span> |
| <span data-ttu-id="b0ace-161">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="b0ace-161">isWheelChairAccessible</span></span> | <span data-ttu-id="b0ace-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0ace-162">Boolean</span></span>                                           | <span data-ttu-id="b0ace-163">Especifica se a sala é acessível para acessibilidade.</span><span class="sxs-lookup"><span data-stu-id="b0ace-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="b0ace-164">rótulo</span><span class="sxs-lookup"><span data-stu-id="b0ace-164">label</span></span>                  | <span data-ttu-id="b0ace-165">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-165">String</span></span>                                            | <span data-ttu-id="b0ace-166">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="b0ace-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="b0ace-167">nickname</span><span class="sxs-lookup"><span data-stu-id="b0ace-167">nickname</span></span>               | <span data-ttu-id="b0ace-168">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-168">String</span></span>                                            | <span data-ttu-id="b0ace-169">Especifica um apelido para a sala, por exemplo, "conf room".</span><span class="sxs-lookup"><span data-stu-id="b0ace-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="b0ace-170">phone</span><span class="sxs-lookup"><span data-stu-id="b0ace-170">phone</span></span>                  | <span data-ttu-id="b0ace-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0ace-171">String</span></span>                                            | <span data-ttu-id="b0ace-172">O número de telefone da sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-172">The phone number of the room.</span></span> |
| <span data-ttu-id="b0ace-173">tags</span><span class="sxs-lookup"><span data-stu-id="b0ace-173">tags</span></span>                   | <span data-ttu-id="b0ace-174">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0ace-174">String collection</span></span>                                 | <span data-ttu-id="b0ace-175">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou o tipo de móveis.</span><span class="sxs-lookup"><span data-stu-id="b0ace-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="b0ace-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="b0ace-176">videoDeviceName</span></span>        | <span data-ttu-id="b0ace-177">String</span><span class="sxs-lookup"><span data-stu-id="b0ace-177">String</span></span>                                            | <span data-ttu-id="b0ace-178">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="b0ace-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="b0ace-179">valores de bookingType</span><span class="sxs-lookup"><span data-stu-id="b0ace-179">bookingType values</span></span>

| <span data-ttu-id="b0ace-180">Valor</span><span class="sxs-lookup"><span data-stu-id="b0ace-180">Value</span></span>    | <span data-ttu-id="b0ace-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ace-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="b0ace-182">padrão</span><span class="sxs-lookup"><span data-stu-id="b0ace-182">standard</span></span> | <span data-ttu-id="b0ace-183">A sala pode ser reservada com base nas outras configurações deste cmdlet.</span><span class="sxs-lookup"><span data-stu-id="b0ace-183">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="b0ace-184">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="b0ace-184">This is the default value.</span></span> |
| <span data-ttu-id="b0ace-185">reservado</span><span class="sxs-lookup"><span data-stu-id="b0ace-185">reserved</span></span> | <span data-ttu-id="b0ace-186">A sala só está disponível por vir, primeiro a ser servido.</span><span class="sxs-lookup"><span data-stu-id="b0ace-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="b0ace-187">Ele não pode ser reservado.</span><span class="sxs-lookup"><span data-stu-id="b0ace-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0ace-188">Relações</span><span class="sxs-lookup"><span data-stu-id="b0ace-188">Relationships</span></span>

<span data-ttu-id="b0ace-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0ace-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0ace-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0ace-190">JSON representation</span></span>

<span data-ttu-id="b0ace-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0ace-191">The following is a JSON representation of the resource.</span></span>

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


