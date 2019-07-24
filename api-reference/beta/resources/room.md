---
title: tipo de recurso Room
description: Especifica as propriedades de uma sala em um locatário.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 41c87daa31feda2907abab6f5711b4b88963095b
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841287"
---
# <a name="room-resource-type"></a><span data-ttu-id="22f4a-103">tipo de recurso Room</span><span class="sxs-lookup"><span data-stu-id="22f4a-103">room resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22f4a-104">Representa uma sala em um locatário.</span><span class="sxs-lookup"><span data-stu-id="22f4a-104">Represents a room in a tenant.</span></span> 

<span data-ttu-id="22f4a-105">No Exchange Online, cada sala é associada a uma caixa de correio de sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-105">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="22f4a-106">Derivado do [local](place.md).</span><span class="sxs-lookup"><span data-stu-id="22f4a-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="22f4a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="22f4a-107">Methods</span></span>

| <span data-ttu-id="22f4a-108">Método</span><span class="sxs-lookup"><span data-stu-id="22f4a-108">Method</span></span>                              | <span data-ttu-id="22f4a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="22f4a-109">Return Type</span></span>                  | <span data-ttu-id="22f4a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="22f4a-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="22f4a-111">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="22f4a-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="22f4a-112">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="22f4a-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="22f4a-113">Obtém uma coleção do tipo especificado do objeto **Place** definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="22f4a-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="22f4a-114">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="22f4a-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="22f4a-115">Obter local</span><span class="sxs-lookup"><span data-stu-id="22f4a-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="22f4a-116">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="22f4a-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="22f4a-117">Obtenha as propriedades e os relacionamentos do objeto **local** especificado, como uma sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-117">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="22f4a-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22f4a-118">Properties</span></span>

| <span data-ttu-id="22f4a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22f4a-119">Property</span></span>               | <span data-ttu-id="22f4a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="22f4a-120">Type</span></span>                                              | <span data-ttu-id="22f4a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="22f4a-121">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="22f4a-122">address</span><span class="sxs-lookup"><span data-stu-id="22f4a-122">address</span></span>                | [<span data-ttu-id="22f4a-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="22f4a-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="22f4a-124">O endereço da sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-124">The street address of the room.</span></span> |
| <span data-ttu-id="22f4a-125">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="22f4a-125">audioDeviceName</span></span>        | <span data-ttu-id="22f4a-126">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-126">String</span></span>                                            | <span data-ttu-id="22f4a-127">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-127">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="22f4a-128">bookingType</span><span class="sxs-lookup"><span data-stu-id="22f4a-128">bookingType</span></span>            | [<span data-ttu-id="22f4a-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="22f4a-129">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="22f4a-130">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-130">Type of room.</span></span> <span data-ttu-id="22f4a-131">Os valores possíveis são: `standard`, `managed` e `reserved`.</span><span class="sxs-lookup"><span data-stu-id="22f4a-131">Possible values are `standard`, `managed`, and `reserved`.</span></span> |
| <span data-ttu-id="22f4a-132">Build</span><span class="sxs-lookup"><span data-stu-id="22f4a-132">building</span></span>               | <span data-ttu-id="22f4a-133">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-133">String</span></span>                                            | <span data-ttu-id="22f4a-134">Especifica o nome do edifício ou o número de edifício em que a sala se encontra.</span><span class="sxs-lookup"><span data-stu-id="22f4a-134">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="22f4a-135">máxima</span><span class="sxs-lookup"><span data-stu-id="22f4a-135">capacity</span></span>               | <span data-ttu-id="22f4a-136">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-136">String</span></span>                                            | <span data-ttu-id="22f4a-137">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-137">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="22f4a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="22f4a-138">displayName</span></span>            | <span data-ttu-id="22f4a-139">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-139">String</span></span>                                            | <span data-ttu-id="22f4a-140">O nome associado à sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-140">The name associated with the room.</span></span> |
| <span data-ttu-id="22f4a-141">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="22f4a-141">displayDeviceName</span></span>      | <span data-ttu-id="22f4a-142">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-142">String</span></span>                                            | <span data-ttu-id="22f4a-143">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-143">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="22f4a-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="22f4a-144">emailAddress</span></span>           | <span data-ttu-id="22f4a-145">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-145">String</span></span>                                            | <span data-ttu-id="22f4a-146">Endereço de email da sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-146">Email address of the room.</span></span> |
| <span data-ttu-id="22f4a-147">floorNumber</span><span class="sxs-lookup"><span data-stu-id="22f4a-147">floorNumber</span></span>            | <span data-ttu-id="22f4a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="22f4a-148">Int32</span></span>                                             | <span data-ttu-id="22f4a-149">Especifica o número do andar em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="22f4a-149">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="22f4a-150">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="22f4a-150">geoCoordinates</span></span>         | [<span data-ttu-id="22f4a-151">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="22f4a-151">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="22f4a-152">Especifica o local da sala no latitude, longitude e, opcionalmente, as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="22f4a-152">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="22f4a-153">id</span><span class="sxs-lookup"><span data-stu-id="22f4a-153">id</span></span>                     | <span data-ttu-id="22f4a-154">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-154">String</span></span>                                            | <span data-ttu-id="22f4a-155">Identificador exclusivo da sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-155">Unique identifier for the room.</span></span> <span data-ttu-id="22f4a-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22f4a-156">Read-only.</span></span> |
| <span data-ttu-id="22f4a-157">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="22f4a-157">isWheelchairAccessible</span></span> | <span data-ttu-id="22f4a-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="22f4a-158">Boolean</span></span>                                           | <span data-ttu-id="22f4a-159">Especifica se a sala pode ser acessada por cadeira.</span><span class="sxs-lookup"><span data-stu-id="22f4a-159">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="22f4a-160">rótulo</span><span class="sxs-lookup"><span data-stu-id="22f4a-160">label</span></span>                  | <span data-ttu-id="22f4a-161">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-161">String</span></span>                                            | <span data-ttu-id="22f4a-162">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="22f4a-162">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="22f4a-163">apelido</span><span class="sxs-lookup"><span data-stu-id="22f4a-163">nickname</span></span>               | <span data-ttu-id="22f4a-164">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-164">String</span></span>                                            | <span data-ttu-id="22f4a-165">Especifica um apelido para a sala, por exemplo, "conf sala".</span><span class="sxs-lookup"><span data-stu-id="22f4a-165">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="22f4a-166">phone</span><span class="sxs-lookup"><span data-stu-id="22f4a-166">phone</span></span>                  | <span data-ttu-id="22f4a-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22f4a-167">String</span></span>                                            | <span data-ttu-id="22f4a-168">O número de telefone da sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-168">The phone number of the room.</span></span> |
| <span data-ttu-id="22f4a-169">marcações</span><span class="sxs-lookup"><span data-stu-id="22f4a-169">tags</span></span>                   | <span data-ttu-id="22f4a-170">String collection</span><span class="sxs-lookup"><span data-stu-id="22f4a-170">String collection</span></span>                                 | <span data-ttu-id="22f4a-171">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou tipo de mobília.</span><span class="sxs-lookup"><span data-stu-id="22f4a-171">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="22f4a-172">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="22f4a-172">videoDeviceName</span></span>        | <span data-ttu-id="22f4a-173">String</span><span class="sxs-lookup"><span data-stu-id="22f4a-173">String</span></span>                                            | <span data-ttu-id="22f4a-174">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="22f4a-174">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="22f4a-175">valores de reserva</span><span class="sxs-lookup"><span data-stu-id="22f4a-175">bookingType values</span></span>

| <span data-ttu-id="22f4a-176">Valor</span><span class="sxs-lookup"><span data-stu-id="22f4a-176">Value</span></span>    | <span data-ttu-id="22f4a-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="22f4a-177">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="22f4a-178">caracteres</span><span class="sxs-lookup"><span data-stu-id="22f4a-178">standard</span></span> | <span data-ttu-id="22f4a-179">A sala pode ser reservada com base nas outras configurações deste cmdlet.</span><span class="sxs-lookup"><span data-stu-id="22f4a-179">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="22f4a-180">O proprietário, o autor e o proprietário do site ainda podem acessar o item.</span><span class="sxs-lookup"><span data-stu-id="22f4a-180">This is the default value.</span></span> |
| <span data-ttu-id="22f4a-181">Managed</span><span class="sxs-lookup"><span data-stu-id="22f4a-181">managed</span></span>  | <span data-ttu-id="22f4a-182">A sala é gerenciada por um representante</span><span class="sxs-lookup"><span data-stu-id="22f4a-182">The room is managed by a delegate</span></span>                         |
| <span data-ttu-id="22f4a-183">serve</span><span class="sxs-lookup"><span data-stu-id="22f4a-183">reserved</span></span> | <span data-ttu-id="22f4a-184">A sala está disponível somente em uma primeira base de chegada.</span><span class="sxs-lookup"><span data-stu-id="22f4a-184">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="22f4a-185">Ele não pode ser reservado.</span><span class="sxs-lookup"><span data-stu-id="22f4a-185">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22f4a-186">Relações</span><span class="sxs-lookup"><span data-stu-id="22f4a-186">Relationships</span></span>

<span data-ttu-id="22f4a-187">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22f4a-187">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="22f4a-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22f4a-188">JSON representation</span></span>

<span data-ttu-id="22f4a-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22f4a-189">The following is a JSON representation of the resource.</span></span>

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
