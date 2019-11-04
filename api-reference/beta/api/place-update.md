---
title: Local de atualização
description: Atualize as propriedades do objeto local.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 5e89dc031802ea420079bbbbbf5dd46f4fe181fc
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949498"
---
# <a name="update-place"></a><span data-ttu-id="a5ffb-103">Local de atualização</span><span class="sxs-lookup"><span data-stu-id="a5ffb-103">Update place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5ffb-104">Atualize as propriedades do objeto [local](../resources/place.md) , que pode ser uma [sala](../resources/room.md) ou uma [sala de salas](../resources/roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="a5ffb-104">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="a5ffb-105">Você pode identificar a **sala** ou a **sala de salas** especificando a propriedade **ID** ou **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="a5ffb-105">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5ffb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5ffb-106">Permissions</span></span>

<span data-ttu-id="a5ffb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5ffb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5ffb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5ffb-109">Permission type</span></span>                        | <span data-ttu-id="a5ffb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5ffb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5ffb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5ffb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5ffb-112">Place. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-112">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="a5ffb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5ffb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5ffb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-114">Not supported.</span></span> |
| <span data-ttu-id="a5ffb-115">Application</span><span class="sxs-lookup"><span data-stu-id="a5ffb-115">Application</span></span>                            | <span data-ttu-id="a5ffb-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a5ffb-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5ffb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5ffb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5ffb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ffb-118">Request headers</span></span>

| <span data-ttu-id="a5ffb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a5ffb-119">Name</span></span>       | <span data-ttu-id="a5ffb-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5ffb-120">Type</span></span> | <span data-ttu-id="a5ffb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ffb-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5ffb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5ffb-122">Authorization</span></span>  | <span data-ttu-id="a5ffb-123">string</span><span class="sxs-lookup"><span data-stu-id="a5ffb-123">string</span></span>  | <span data-ttu-id="a5ffb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5ffb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ffb-126">Request body</span></span>

<span data-ttu-id="a5ffb-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a5ffb-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a5ffb-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a5ffb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5ffb-130">Property</span></span>               | <span data-ttu-id="a5ffb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5ffb-131">Type</span></span>                                              | <span data-ttu-id="a5ffb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ffb-132">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="a5ffb-133">address</span><span class="sxs-lookup"><span data-stu-id="a5ffb-133">address</span></span>                | [<span data-ttu-id="a5ffb-134">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a5ffb-134">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="a5ffb-135">O endereço da sala ou da sala de salas.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-135">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="a5ffb-136">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="a5ffb-136">audioDeviceName</span></span>        | <span data-ttu-id="a5ffb-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-137">String</span></span>                                            | <span data-ttu-id="a5ffb-138">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-138">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="a5ffb-139">bookingType</span><span class="sxs-lookup"><span data-stu-id="a5ffb-139">bookingType</span></span>            | [<span data-ttu-id="a5ffb-140">bookingType</span><span class="sxs-lookup"><span data-stu-id="a5ffb-140">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="a5ffb-141">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-141">Type of room.</span></span> <span data-ttu-id="a5ffb-142">Os valores possíveis são: `Standard` e `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-142">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="a5ffb-143">Build</span><span class="sxs-lookup"><span data-stu-id="a5ffb-143">building</span></span>               | <span data-ttu-id="a5ffb-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-144">String</span></span>                                            | <span data-ttu-id="a5ffb-145">Especifica o nome do edifício ou o número de edifício em que a sala se encontra.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-145">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="a5ffb-146">máxima</span><span class="sxs-lookup"><span data-stu-id="a5ffb-146">capacity</span></span>               | <span data-ttu-id="a5ffb-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-147">String</span></span>                                            | <span data-ttu-id="a5ffb-148">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-148">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="a5ffb-149">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="a5ffb-149">displayDeviceName</span></span>      | <span data-ttu-id="a5ffb-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-150">String</span></span>                                            | <span data-ttu-id="a5ffb-151">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-151">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="a5ffb-152">floorLabel</span><span class="sxs-lookup"><span data-stu-id="a5ffb-152">floorLabel</span></span>             | <span data-ttu-id="a5ffb-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-153">String</span></span>                                            | <span data-ttu-id="a5ffb-154">Especifica a carta de piso em que a sala está ativa.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-154">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="a5ffb-155">floorNumber</span><span class="sxs-lookup"><span data-stu-id="a5ffb-155">floorNumber</span></span>            | <span data-ttu-id="a5ffb-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a5ffb-156">Int32</span></span>                                             | <span data-ttu-id="a5ffb-157">Especifica o número do andar em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-157">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="a5ffb-158">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a5ffb-158">geoCoordinates</span></span>         | [<span data-ttu-id="a5ffb-159">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a5ffb-159">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="a5ffb-160">Especifica o local da sala ou da sala de opções no latitude, longitude e, opcionalmente, as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-160">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="a5ffb-161">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="a5ffb-161">isWheelchairAccessible</span></span> | <span data-ttu-id="a5ffb-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5ffb-162">Boolean</span></span>                                           | <span data-ttu-id="a5ffb-163">Especifica se a sala pode ser acessada por cadeira.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="a5ffb-164">rótulo</span><span class="sxs-lookup"><span data-stu-id="a5ffb-164">label</span></span>                  | <span data-ttu-id="a5ffb-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-165">String</span></span>                                            | <span data-ttu-id="a5ffb-166">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="a5ffb-167">apelido</span><span class="sxs-lookup"><span data-stu-id="a5ffb-167">nickname</span></span>               | <span data-ttu-id="a5ffb-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-168">String</span></span>                                            | <span data-ttu-id="a5ffb-169">Especifica um apelido para a sala, por exemplo, "conf sala".</span><span class="sxs-lookup"><span data-stu-id="a5ffb-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="a5ffb-170">phone</span><span class="sxs-lookup"><span data-stu-id="a5ffb-170">phone</span></span>                  | <span data-ttu-id="a5ffb-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-171">String</span></span>                                            | <span data-ttu-id="a5ffb-172">O número de telefone da sala ou sala de salas.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-172">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="a5ffb-173">tags</span><span class="sxs-lookup"><span data-stu-id="a5ffb-173">tags</span></span>                   | <span data-ttu-id="a5ffb-174">String collection</span><span class="sxs-lookup"><span data-stu-id="a5ffb-174">String collection</span></span>                                 | <span data-ttu-id="a5ffb-175">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou tipo de mobília.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="a5ffb-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="a5ffb-176">videoDeviceName</span></span>        | <span data-ttu-id="a5ffb-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ffb-177">String</span></span>                                            | <span data-ttu-id="a5ffb-178">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-178">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="a5ffb-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ffb-179">Response</span></span>

<span data-ttu-id="a5ffb-180">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Place](../resources/place.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-180">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5ffb-181">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5ffb-181">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="a5ffb-182">Exemplo 1: atualizar uma sala</span><span class="sxs-lookup"><span data-stu-id="a5ffb-182">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="a5ffb-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ffb-183">Request</span></span>

<span data-ttu-id="a5ffb-184">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-184">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "update_room"
}-->
```http
PATCH https://graph.microsoft.com/beta/places/cf100@contoso.com
Content-type: application/json
Content-length: 285

{
  "@odata.type": "microsoft.graph.room",
  "nickname": "Conf Room",
  "building": "1",
  "label": "100",
  "capacity": "50",
  "isWheelchairAccessible": false
}
```

### <a name="response"></a><span data-ttu-id="a5ffb-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ffb-185">Response</span></span>

<span data-ttu-id="a5ffb-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-186">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a5ffb-187">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-187">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5ffb-188">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-188">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
    "@odata.type": "#microsoft.graph.room",
    "id": "3162F1E1-C4C0-604B-51D8-91DA78989EB1",
    "emailAddress": "cf100@contoso.com",
    "displayName": "Conf Room 100",
    "address": {
      "street": "4567 Main Street",
      "city": "Buffalo",
      "state": "NY",
      "postalCode": "98052",
      "countryOrRegion": "USA"
    },
    "geoCoordinates": {
      "latitude": 47.640568390488626,
      "longitude": -122.1293731033803
    },
    "phone": "555-555-0100",
    "nickname": "Conf Room",
    "label": "100",
    "capacity": "50",
    "building": "1",
    "floorLabel": "1P",
    "floorNumber": 1,
    "isManaged": true,
    "isWheelchairAccessible": false,
    "bookingType": "standard",
    "tags": [
      "bean bags"
    ],
    "audioDeviceName": null,
    "videoDeviceName": null,
    "displayDevice": "surface hub"
}
```

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="a5ffb-189">Exemplo 2: atualizar uma salalist</span><span class="sxs-lookup"><span data-stu-id="a5ffb-189">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="a5ffb-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ffb-190">Request</span></span>

<span data-ttu-id="a5ffb-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-191">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/beta/places/Building1RroomList@contoso.onmicrosoft.com
Content-type: application/json

{
  "@odata.type": "microsoft.graph.roomlist",
  "displayName": "Building 1",
  "phone":"555-555-0100"
}
```

### <a name="response"></a><span data-ttu-id="a5ffb-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ffb-192">Response</span></span>

<span data-ttu-id="a5ffb-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-193">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a5ffb-194">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-194">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5ffb-195">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5ffb-195">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
  "@odata.type": "#microsoft.graph.roomList",
  "id": "DC404124-302A-92AA-F98D-7B4DEB0C1705",
  "displayName": "Building 1",
  "address": {
    "street": "4567 Main Street",
    "city": "Buffalo",
    "state": "NY",
    "postalCode": "98052",
    "countryOrRegion": "USA"
  },
  "geocoordinates": null,
  "phone": "555-555-0100",
  "emailAddress": "bldg1@contoso.com"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
