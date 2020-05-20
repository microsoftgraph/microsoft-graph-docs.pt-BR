---
title: tipo de recurso Room
description: Especifica as propriedades de uma sala em um locatário.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a2ae65132e368faa12517e13a0fbd5e65572cde4
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290557"
---
# <a name="room-resource-type"></a><span data-ttu-id="91ecb-103">tipo de recurso Room</span><span class="sxs-lookup"><span data-stu-id="91ecb-103">room resource type</span></span>

<span data-ttu-id="91ecb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91ecb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91ecb-105">Representa uma sala em um locatário.</span><span class="sxs-lookup"><span data-stu-id="91ecb-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="91ecb-106">No Exchange Online, cada sala é associada a uma caixa de correio de sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="91ecb-107">Derivado do [local](place.md).</span><span class="sxs-lookup"><span data-stu-id="91ecb-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="91ecb-108">Methods</span><span class="sxs-lookup"><span data-stu-id="91ecb-108">Methods</span></span>

| <span data-ttu-id="91ecb-109">Método</span><span class="sxs-lookup"><span data-stu-id="91ecb-109">Method</span></span>                              | <span data-ttu-id="91ecb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="91ecb-110">Return Type</span></span>                  | <span data-ttu-id="91ecb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="91ecb-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="91ecb-112">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="91ecb-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="91ecb-113">Uma coleção do tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="91ecb-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="91ecb-114">Obtém uma coleção do tipo especificado do objeto **Place** definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="91ecb-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="91ecb-115">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="91ecb-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="91ecb-116">Obter local</span><span class="sxs-lookup"><span data-stu-id="91ecb-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="91ecb-117">O tipo de [local](place.md) solicitado e derivado</span><span class="sxs-lookup"><span data-stu-id="91ecb-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="91ecb-118">Obtenha as propriedades e os relacionamentos do objeto **local** especificado, como uma sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="91ecb-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91ecb-119">Properties</span></span>

| <span data-ttu-id="91ecb-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91ecb-120">Property</span></span>               | <span data-ttu-id="91ecb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="91ecb-121">Type</span></span>                                              | <span data-ttu-id="91ecb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="91ecb-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="91ecb-123">address</span><span class="sxs-lookup"><span data-stu-id="91ecb-123">address</span></span>                | [<span data-ttu-id="91ecb-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="91ecb-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="91ecb-125">O endereço da sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-125">The street address of the room.</span></span> |
| <span data-ttu-id="91ecb-126">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="91ecb-126">audioDeviceName</span></span>        | <span data-ttu-id="91ecb-127">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-127">String</span></span>                                            | <span data-ttu-id="91ecb-128">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="91ecb-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="91ecb-129">bookingType</span></span>            | [<span data-ttu-id="91ecb-130">bookingType</span><span class="sxs-lookup"><span data-stu-id="91ecb-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="91ecb-131">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-131">Type of room.</span></span> <span data-ttu-id="91ecb-132">Os valores possíveis são `standard` e `reserved` .</span><span class="sxs-lookup"><span data-stu-id="91ecb-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="91ecb-133">Build</span><span class="sxs-lookup"><span data-stu-id="91ecb-133">building</span></span>               | <span data-ttu-id="91ecb-134">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-134">String</span></span>                                            | <span data-ttu-id="91ecb-135">Especifica o nome do edifício ou o número de edifício em que a sala se encontra.</span><span class="sxs-lookup"><span data-stu-id="91ecb-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="91ecb-136">máxima</span><span class="sxs-lookup"><span data-stu-id="91ecb-136">capacity</span></span>               | <span data-ttu-id="91ecb-137">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-137">String</span></span>                                            | <span data-ttu-id="91ecb-138">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="91ecb-139">displayName</span><span class="sxs-lookup"><span data-stu-id="91ecb-139">displayName</span></span>            | <span data-ttu-id="91ecb-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ecb-140">String</span></span>                                            | <span data-ttu-id="91ecb-141">O nome associado à sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-141">The name associated with the room.</span></span> |
| <span data-ttu-id="91ecb-142">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="91ecb-142">displayDeviceName</span></span>      | <span data-ttu-id="91ecb-143">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-143">String</span></span>                                            | <span data-ttu-id="91ecb-144">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="91ecb-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="91ecb-145">emailAddress</span></span>           | <span data-ttu-id="91ecb-146">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-146">String</span></span>                                            | <span data-ttu-id="91ecb-147">Endereço de email da sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-147">Email address of the room.</span></span> |
| <span data-ttu-id="91ecb-148">floorLabel</span><span class="sxs-lookup"><span data-stu-id="91ecb-148">floorLabel</span></span>             | <span data-ttu-id="91ecb-149">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-149">String</span></span>                                            | <span data-ttu-id="91ecb-150">Especifica um rótulo descritivo para o andar, por exemplo, P.</span><span class="sxs-lookup"><span data-stu-id="91ecb-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="91ecb-151">floorNumber</span><span class="sxs-lookup"><span data-stu-id="91ecb-151">floorNumber</span></span>            | <span data-ttu-id="91ecb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="91ecb-152">Int32</span></span>                                             | <span data-ttu-id="91ecb-153">Especifica o número do andar em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="91ecb-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="91ecb-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="91ecb-154">geoCoordinates</span></span>         | [<span data-ttu-id="91ecb-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="91ecb-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="91ecb-156">Especifica o local da sala no latitude, longitude e, opcionalmente, as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="91ecb-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="91ecb-157">id</span><span class="sxs-lookup"><span data-stu-id="91ecb-157">id</span></span>                     | <span data-ttu-id="91ecb-158">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-158">String</span></span>                                            | <span data-ttu-id="91ecb-159">Identificador exclusivo da sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-159">Unique identifier for the room.</span></span> <span data-ttu-id="91ecb-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91ecb-160">Read-only.</span></span> |
| <span data-ttu-id="91ecb-161">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="91ecb-161">isWheelchairAccessible</span></span> | <span data-ttu-id="91ecb-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="91ecb-162">Boolean</span></span>                                           | <span data-ttu-id="91ecb-163">Especifica se a sala pode ser acessada por cadeira.</span><span class="sxs-lookup"><span data-stu-id="91ecb-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="91ecb-164">rótulo</span><span class="sxs-lookup"><span data-stu-id="91ecb-164">label</span></span>                  | <span data-ttu-id="91ecb-165">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-165">String</span></span>                                            | <span data-ttu-id="91ecb-166">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="91ecb-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="91ecb-167">apelido</span><span class="sxs-lookup"><span data-stu-id="91ecb-167">nickname</span></span>               | <span data-ttu-id="91ecb-168">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-168">String</span></span>                                            | <span data-ttu-id="91ecb-169">Especifica um apelido para a sala, por exemplo, "conf sala".</span><span class="sxs-lookup"><span data-stu-id="91ecb-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="91ecb-170">phone</span><span class="sxs-lookup"><span data-stu-id="91ecb-170">phone</span></span>                  | <span data-ttu-id="91ecb-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ecb-171">String</span></span>                                            | <span data-ttu-id="91ecb-172">O número de telefone da sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-172">The phone number of the room.</span></span> |
| <span data-ttu-id="91ecb-173">tags</span><span class="sxs-lookup"><span data-stu-id="91ecb-173">tags</span></span>                   | <span data-ttu-id="91ecb-174">String collection</span><span class="sxs-lookup"><span data-stu-id="91ecb-174">String collection</span></span>                                 | <span data-ttu-id="91ecb-175">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou tipo de mobília.</span><span class="sxs-lookup"><span data-stu-id="91ecb-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="91ecb-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="91ecb-176">videoDeviceName</span></span>        | <span data-ttu-id="91ecb-177">String</span><span class="sxs-lookup"><span data-stu-id="91ecb-177">String</span></span>                                            | <span data-ttu-id="91ecb-178">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="91ecb-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="91ecb-179">valores de reserva</span><span class="sxs-lookup"><span data-stu-id="91ecb-179">bookingType values</span></span>

| <span data-ttu-id="91ecb-180">Valor</span><span class="sxs-lookup"><span data-stu-id="91ecb-180">Value</span></span>    | <span data-ttu-id="91ecb-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="91ecb-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="91ecb-182">caracteres</span><span class="sxs-lookup"><span data-stu-id="91ecb-182">standard</span></span> | <span data-ttu-id="91ecb-183">A sala está disponível e pode ser reservada.</span><span class="sxs-lookup"><span data-stu-id="91ecb-183">The room is available and can be reserved.</span></span> <span data-ttu-id="91ecb-184">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="91ecb-184">This is the default value.</span></span> |
| <span data-ttu-id="91ecb-185">serve</span><span class="sxs-lookup"><span data-stu-id="91ecb-185">reserved</span></span> | <span data-ttu-id="91ecb-186">A sala está disponível somente em uma primeira base de chegada.</span><span class="sxs-lookup"><span data-stu-id="91ecb-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="91ecb-187">Ele não pode ser reservado.</span><span class="sxs-lookup"><span data-stu-id="91ecb-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91ecb-188">Relações</span><span class="sxs-lookup"><span data-stu-id="91ecb-188">Relationships</span></span>

<span data-ttu-id="91ecb-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91ecb-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="91ecb-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91ecb-190">JSON representation</span></span>

<span data-ttu-id="91ecb-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91ecb-191">The following is a JSON representation of the resource.</span></span>

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
