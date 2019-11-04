---
title: tipo de recurso Room
description: Especifica as propriedades de uma sala em um locatário.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: cfa1d87093c7f843dd9a8294a253751726b3d34b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938720"
---
# <a name="room-resource-type"></a><span data-ttu-id="1d652-103">tipo de recurso Room</span><span class="sxs-lookup"><span data-stu-id="1d652-103">room resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d652-104">Representa uma sala em um locatário.</span><span class="sxs-lookup"><span data-stu-id="1d652-104">Represents a room in a tenant.</span></span> 

<span data-ttu-id="1d652-105">No Exchange Online, cada sala é associada a uma caixa de correio de sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-105">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="1d652-106">Derivado do [local](place.md).</span><span class="sxs-lookup"><span data-stu-id="1d652-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1d652-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d652-107">Methods</span></span>

| <span data-ttu-id="1d652-108">Método</span><span class="sxs-lookup"><span data-stu-id="1d652-108">Method</span></span>                              | <span data-ttu-id="1d652-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d652-109">Return Type</span></span>                  | <span data-ttu-id="1d652-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d652-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="1d652-111">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="1d652-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="1d652-112">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="1d652-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="1d652-113">Obtém uma coleção do tipo especificado do objeto **Place** definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="1d652-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="1d652-114">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="1d652-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="1d652-115">Obter local</span><span class="sxs-lookup"><span data-stu-id="1d652-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="1d652-116">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="1d652-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="1d652-117">Obtenha as propriedades e os relacionamentos do objeto **local** especificado, como uma sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-117">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d652-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d652-118">Properties</span></span>

| <span data-ttu-id="1d652-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d652-119">Property</span></span>               | <span data-ttu-id="1d652-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d652-120">Type</span></span>                                              | <span data-ttu-id="1d652-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d652-121">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="1d652-122">address</span><span class="sxs-lookup"><span data-stu-id="1d652-122">address</span></span>                | [<span data-ttu-id="1d652-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="1d652-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="1d652-124">O endereço da sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-124">The street address of the room.</span></span> |
| <span data-ttu-id="1d652-125">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="1d652-125">audioDeviceName</span></span>        | <span data-ttu-id="1d652-126">String</span><span class="sxs-lookup"><span data-stu-id="1d652-126">String</span></span>                                            | <span data-ttu-id="1d652-127">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-127">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="1d652-128">bookingType</span><span class="sxs-lookup"><span data-stu-id="1d652-128">bookingType</span></span>            | [<span data-ttu-id="1d652-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="1d652-129">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="1d652-130">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-130">Type of room.</span></span> <span data-ttu-id="1d652-131">Os valores possíveis `standard`são e `reserved`.</span><span class="sxs-lookup"><span data-stu-id="1d652-131">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="1d652-132">Build</span><span class="sxs-lookup"><span data-stu-id="1d652-132">building</span></span>               | <span data-ttu-id="1d652-133">String</span><span class="sxs-lookup"><span data-stu-id="1d652-133">String</span></span>                                            | <span data-ttu-id="1d652-134">Especifica o nome do edifício ou o número de edifício em que a sala se encontra.</span><span class="sxs-lookup"><span data-stu-id="1d652-134">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="1d652-135">máxima</span><span class="sxs-lookup"><span data-stu-id="1d652-135">capacity</span></span>               | <span data-ttu-id="1d652-136">String</span><span class="sxs-lookup"><span data-stu-id="1d652-136">String</span></span>                                            | <span data-ttu-id="1d652-137">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-137">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="1d652-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1d652-138">displayName</span></span>            | <span data-ttu-id="1d652-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d652-139">String</span></span>                                            | <span data-ttu-id="1d652-140">O nome associado à sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-140">The name associated with the room.</span></span> |
| <span data-ttu-id="1d652-141">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="1d652-141">displayDeviceName</span></span>      | <span data-ttu-id="1d652-142">String</span><span class="sxs-lookup"><span data-stu-id="1d652-142">String</span></span>                                            | <span data-ttu-id="1d652-143">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-143">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="1d652-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1d652-144">emailAddress</span></span>           | <span data-ttu-id="1d652-145">String</span><span class="sxs-lookup"><span data-stu-id="1d652-145">String</span></span>                                            | <span data-ttu-id="1d652-146">Endereço de email da sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-146">Email address of the room.</span></span> |
| <span data-ttu-id="1d652-147">floorLabel</span><span class="sxs-lookup"><span data-stu-id="1d652-147">floorLabel</span></span>             | <span data-ttu-id="1d652-148">String</span><span class="sxs-lookup"><span data-stu-id="1d652-148">String</span></span>                                            | <span data-ttu-id="1d652-149">Especifica um rótulo descritivo para o andar, por exemplo, P.</span><span class="sxs-lookup"><span data-stu-id="1d652-149">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="1d652-150">floorNumber</span><span class="sxs-lookup"><span data-stu-id="1d652-150">floorNumber</span></span>            | <span data-ttu-id="1d652-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1d652-151">Int32</span></span>                                             | <span data-ttu-id="1d652-152">Especifica o número do andar em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="1d652-152">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="1d652-153">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="1d652-153">geoCoordinates</span></span>         | [<span data-ttu-id="1d652-154">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="1d652-154">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="1d652-155">Especifica o local da sala no latitude, longitude e, opcionalmente, as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="1d652-155">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="1d652-156">id</span><span class="sxs-lookup"><span data-stu-id="1d652-156">id</span></span>                     | <span data-ttu-id="1d652-157">String</span><span class="sxs-lookup"><span data-stu-id="1d652-157">String</span></span>                                            | <span data-ttu-id="1d652-158">Identificador exclusivo da sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-158">Unique identifier for the room.</span></span> <span data-ttu-id="1d652-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d652-159">Read-only.</span></span> |
| <span data-ttu-id="1d652-160">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="1d652-160">isWheelchairAccessible</span></span> | <span data-ttu-id="1d652-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d652-161">Boolean</span></span>                                           | <span data-ttu-id="1d652-162">Especifica se a sala pode ser acessada por cadeira.</span><span class="sxs-lookup"><span data-stu-id="1d652-162">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="1d652-163">rótulo</span><span class="sxs-lookup"><span data-stu-id="1d652-163">label</span></span>                  | <span data-ttu-id="1d652-164">String</span><span class="sxs-lookup"><span data-stu-id="1d652-164">String</span></span>                                            | <span data-ttu-id="1d652-165">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="1d652-165">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="1d652-166">apelido</span><span class="sxs-lookup"><span data-stu-id="1d652-166">nickname</span></span>               | <span data-ttu-id="1d652-167">String</span><span class="sxs-lookup"><span data-stu-id="1d652-167">String</span></span>                                            | <span data-ttu-id="1d652-168">Especifica um apelido para a sala, por exemplo, "conf sala".</span><span class="sxs-lookup"><span data-stu-id="1d652-168">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="1d652-169">phone</span><span class="sxs-lookup"><span data-stu-id="1d652-169">phone</span></span>                  | <span data-ttu-id="1d652-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d652-170">String</span></span>                                            | <span data-ttu-id="1d652-171">O número de telefone da sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-171">The phone number of the room.</span></span> |
| <span data-ttu-id="1d652-172">tags</span><span class="sxs-lookup"><span data-stu-id="1d652-172">tags</span></span>                   | <span data-ttu-id="1d652-173">String collection</span><span class="sxs-lookup"><span data-stu-id="1d652-173">String collection</span></span>                                 | <span data-ttu-id="1d652-174">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou tipo de mobília.</span><span class="sxs-lookup"><span data-stu-id="1d652-174">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="1d652-175">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="1d652-175">videoDeviceName</span></span>        | <span data-ttu-id="1d652-176">String</span><span class="sxs-lookup"><span data-stu-id="1d652-176">String</span></span>                                            | <span data-ttu-id="1d652-177">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="1d652-177">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="1d652-178">valores de reserva</span><span class="sxs-lookup"><span data-stu-id="1d652-178">bookingType values</span></span>

| <span data-ttu-id="1d652-179">Valor</span><span class="sxs-lookup"><span data-stu-id="1d652-179">Value</span></span>    | <span data-ttu-id="1d652-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d652-180">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="1d652-181">caracteres</span><span class="sxs-lookup"><span data-stu-id="1d652-181">standard</span></span> | <span data-ttu-id="1d652-182">A sala pode ser reservada com base nas outras configurações deste cmdlet.</span><span class="sxs-lookup"><span data-stu-id="1d652-182">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="1d652-183">O proprietário, o autor e o proprietário do site ainda podem acessar o item.</span><span class="sxs-lookup"><span data-stu-id="1d652-183">This is the default value.</span></span> |
| <span data-ttu-id="1d652-184">serve</span><span class="sxs-lookup"><span data-stu-id="1d652-184">reserved</span></span> | <span data-ttu-id="1d652-185">A sala está disponível somente em uma primeira base de chegada.</span><span class="sxs-lookup"><span data-stu-id="1d652-185">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="1d652-186">Ele não pode ser reservado.</span><span class="sxs-lookup"><span data-stu-id="1d652-186">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d652-187">Relações</span><span class="sxs-lookup"><span data-stu-id="1d652-187">Relationships</span></span>

<span data-ttu-id="1d652-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d652-188">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d652-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d652-189">JSON representation</span></span>

<span data-ttu-id="1d652-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d652-190">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "String",
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelchairAccessible": true,
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
