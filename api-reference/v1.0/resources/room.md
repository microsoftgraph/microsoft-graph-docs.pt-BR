---
title: tipo de recurso Room
description: Especifica as propriedades de uma sala em um locatário.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 14067f71ae338ae0da026c98d6732fc2ae4eaf57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094173"
---
# <a name="room-resource-type"></a><span data-ttu-id="57a29-103">tipo de recurso Room</span><span class="sxs-lookup"><span data-stu-id="57a29-103">room resource type</span></span>

<span data-ttu-id="57a29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57a29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57a29-105">Representa uma sala em um locatário.</span><span class="sxs-lookup"><span data-stu-id="57a29-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="57a29-106">No Exchange Online, cada sala é associada a uma caixa de correio de sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="57a29-107">Derivado do [local](place.md).</span><span class="sxs-lookup"><span data-stu-id="57a29-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="57a29-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="57a29-108">Methods</span></span>

| <span data-ttu-id="57a29-109">Método</span><span class="sxs-lookup"><span data-stu-id="57a29-109">Method</span></span>                              | <span data-ttu-id="57a29-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="57a29-110">Return Type</span></span>                  | <span data-ttu-id="57a29-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="57a29-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="57a29-112">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="57a29-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="57a29-113">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="57a29-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="57a29-114">Obtém uma coleção do tipo especificado do objeto **Place** definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="57a29-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="57a29-115">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="57a29-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="57a29-116">Obter local</span><span class="sxs-lookup"><span data-stu-id="57a29-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="57a29-117">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="57a29-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="57a29-118">Obtenha as propriedades e os relacionamentos do objeto **local** especificado, como uma sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="57a29-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57a29-119">Properties</span></span>

| <span data-ttu-id="57a29-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57a29-120">Property</span></span>               | <span data-ttu-id="57a29-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="57a29-121">Type</span></span>                                              | <span data-ttu-id="57a29-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="57a29-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="57a29-123">address</span><span class="sxs-lookup"><span data-stu-id="57a29-123">address</span></span>                | [<span data-ttu-id="57a29-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="57a29-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="57a29-125">O endereço da sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-125">The street address of the room.</span></span> |
| <span data-ttu-id="57a29-126">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="57a29-126">audioDeviceName</span></span>        | <span data-ttu-id="57a29-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-127">String</span></span>                                            | <span data-ttu-id="57a29-128">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="57a29-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="57a29-129">bookingType</span></span>            | [<span data-ttu-id="57a29-130">bookingType</span><span class="sxs-lookup"><span data-stu-id="57a29-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="57a29-131">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-131">Type of room.</span></span> <span data-ttu-id="57a29-132">Os valores possíveis são `standard` e `reserved` .</span><span class="sxs-lookup"><span data-stu-id="57a29-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="57a29-133">Build</span><span class="sxs-lookup"><span data-stu-id="57a29-133">building</span></span>               | <span data-ttu-id="57a29-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-134">String</span></span>                                            | <span data-ttu-id="57a29-135">Especifica o nome do edifício ou o número de edifício em que a sala se encontra.</span><span class="sxs-lookup"><span data-stu-id="57a29-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="57a29-136">máxima</span><span class="sxs-lookup"><span data-stu-id="57a29-136">capacity</span></span>               | <span data-ttu-id="57a29-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-137">String</span></span>                                            | <span data-ttu-id="57a29-138">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="57a29-139">displayName</span><span class="sxs-lookup"><span data-stu-id="57a29-139">displayName</span></span>            | <span data-ttu-id="57a29-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-140">String</span></span>                                            | <span data-ttu-id="57a29-141">O nome associado à sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-141">The name associated with the room.</span></span> |
| <span data-ttu-id="57a29-142">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="57a29-142">displayDeviceName</span></span>      | <span data-ttu-id="57a29-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-143">String</span></span>                                            | <span data-ttu-id="57a29-144">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="57a29-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="57a29-145">emailAddress</span></span>           | <span data-ttu-id="57a29-146">String</span><span class="sxs-lookup"><span data-stu-id="57a29-146">String</span></span>                                            | <span data-ttu-id="57a29-147">Endereço de email da sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-147">Email address of the room.</span></span> |
| <span data-ttu-id="57a29-148">floorLabel</span><span class="sxs-lookup"><span data-stu-id="57a29-148">floorLabel</span></span>             | <span data-ttu-id="57a29-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-149">String</span></span>                                            | <span data-ttu-id="57a29-150">Especifica um rótulo descritivo para o andar, por exemplo, P.</span><span class="sxs-lookup"><span data-stu-id="57a29-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="57a29-151">floorNumber</span><span class="sxs-lookup"><span data-stu-id="57a29-151">floorNumber</span></span>            | <span data-ttu-id="57a29-152">Int32</span><span class="sxs-lookup"><span data-stu-id="57a29-152">Int32</span></span>                                             | <span data-ttu-id="57a29-153">Especifica o número do andar em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="57a29-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="57a29-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="57a29-154">geoCoordinates</span></span>         | [<span data-ttu-id="57a29-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="57a29-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="57a29-156">Especifica o local da sala no latitude, longitude e, opcionalmente, as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="57a29-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="57a29-157">id</span><span class="sxs-lookup"><span data-stu-id="57a29-157">id</span></span>                     | <span data-ttu-id="57a29-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-158">String</span></span>                                            | <span data-ttu-id="57a29-159">Identificador exclusivo da sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-159">Unique identifier for the room.</span></span> <span data-ttu-id="57a29-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="57a29-160">Read-only.</span></span> |
| <span data-ttu-id="57a29-161">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="57a29-161">isWheelchairAccessible</span></span> | <span data-ttu-id="57a29-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="57a29-162">Boolean</span></span>                                           | <span data-ttu-id="57a29-163">Especifica se a sala pode ser acessada por cadeira.</span><span class="sxs-lookup"><span data-stu-id="57a29-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="57a29-164">rótulo</span><span class="sxs-lookup"><span data-stu-id="57a29-164">label</span></span>                  | <span data-ttu-id="57a29-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-165">String</span></span>                                            | <span data-ttu-id="57a29-166">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="57a29-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="57a29-167">apelido</span><span class="sxs-lookup"><span data-stu-id="57a29-167">nickname</span></span>               | <span data-ttu-id="57a29-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-168">String</span></span>                                            | <span data-ttu-id="57a29-169">Especifica um apelido para a sala, por exemplo, "conf sala".</span><span class="sxs-lookup"><span data-stu-id="57a29-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="57a29-170">phone</span><span class="sxs-lookup"><span data-stu-id="57a29-170">phone</span></span>                  | <span data-ttu-id="57a29-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-171">String</span></span>                                            | <span data-ttu-id="57a29-172">O número de telefone da sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-172">The phone number of the room.</span></span> |
| <span data-ttu-id="57a29-173">tags</span><span class="sxs-lookup"><span data-stu-id="57a29-173">tags</span></span>                   | <span data-ttu-id="57a29-174">Coleção String</span><span class="sxs-lookup"><span data-stu-id="57a29-174">String collection</span></span>                                 | <span data-ttu-id="57a29-175">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou tipo de mobília.</span><span class="sxs-lookup"><span data-stu-id="57a29-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="57a29-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="57a29-176">videoDeviceName</span></span>        | <span data-ttu-id="57a29-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-177">String</span></span>                                            | <span data-ttu-id="57a29-178">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="57a29-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="57a29-179">valores de reserva</span><span class="sxs-lookup"><span data-stu-id="57a29-179">bookingType values</span></span>

| <span data-ttu-id="57a29-180">Valor</span><span class="sxs-lookup"><span data-stu-id="57a29-180">Value</span></span>    | <span data-ttu-id="57a29-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="57a29-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="57a29-182">caracteres</span><span class="sxs-lookup"><span data-stu-id="57a29-182">standard</span></span> | <span data-ttu-id="57a29-183">A sala está disponível e pode ser reservada.</span><span class="sxs-lookup"><span data-stu-id="57a29-183">The room is available and can be reserved.</span></span> <span data-ttu-id="57a29-184">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="57a29-184">This is the default value.</span></span> |
| <span data-ttu-id="57a29-185">serve</span><span class="sxs-lookup"><span data-stu-id="57a29-185">reserved</span></span> | <span data-ttu-id="57a29-186">A sala está disponível somente em uma primeira base de chegada.</span><span class="sxs-lookup"><span data-stu-id="57a29-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="57a29-187">Ele não pode ser reservado.</span><span class="sxs-lookup"><span data-stu-id="57a29-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57a29-188">Relações</span><span class="sxs-lookup"><span data-stu-id="57a29-188">Relationships</span></span>

<span data-ttu-id="57a29-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57a29-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57a29-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57a29-190">JSON representation</span></span>

<span data-ttu-id="57a29-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57a29-191">The following is a JSON representation of the resource.</span></span>

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

