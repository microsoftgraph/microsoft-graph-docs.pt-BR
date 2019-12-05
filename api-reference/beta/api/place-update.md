---
title: Local de atualização
description: Atualize as propriedades do objeto local.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 3e2e517d0a20384c8aaaa24e9f385cf5560c411e
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844187"
---
# <a name="update-place"></a><span data-ttu-id="59201-103">Local de atualização</span><span class="sxs-lookup"><span data-stu-id="59201-103">Update place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59201-104">Atualize as propriedades do objeto [local](../resources/place.md) , que pode ser uma [sala](../resources/room.md) ou uma [sala de salas](../resources/roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="59201-104">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="59201-105">Você pode identificar a **sala** ou a **sala de salas** especificando a propriedade **ID** ou **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="59201-105">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="59201-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59201-106">Permissions</span></span>

<span data-ttu-id="59201-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59201-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59201-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59201-109">Permission type</span></span>                        | <span data-ttu-id="59201-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59201-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="59201-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59201-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="59201-112">Place. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="59201-112">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="59201-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59201-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59201-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59201-114">Not supported.</span></span> |
| <span data-ttu-id="59201-115">Application</span><span class="sxs-lookup"><span data-stu-id="59201-115">Application</span></span>                            | <span data-ttu-id="59201-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59201-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="59201-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59201-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="59201-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59201-118">Request headers</span></span>

| <span data-ttu-id="59201-119">Nome</span><span class="sxs-lookup"><span data-stu-id="59201-119">Name</span></span>       | <span data-ttu-id="59201-120">Valor</span><span class="sxs-lookup"><span data-stu-id="59201-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="59201-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="59201-121">Authorization</span></span>  | <span data-ttu-id="59201-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59201-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59201-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59201-124">Content-Type</span></span> | <span data-ttu-id="59201-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59201-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59201-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59201-127">Request body</span></span>

<span data-ttu-id="59201-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="59201-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="59201-129">Somente uma instância de um recurso de colocar (**sala** ou **sala de salas**) pode ser atualizada de cada vez.</span><span class="sxs-lookup"><span data-stu-id="59201-129">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="59201-130">No corpo da solicitação, use `@odata.type` para especificar o tipo de local e inclua as propriedades desse tipo para atualizar.</span><span class="sxs-lookup"><span data-stu-id="59201-130">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="59201-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="59201-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="59201-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="59201-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59201-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59201-133">Property</span></span>               | <span data-ttu-id="59201-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="59201-134">Type</span></span>                                              | <span data-ttu-id="59201-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="59201-135">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="59201-136">address</span><span class="sxs-lookup"><span data-stu-id="59201-136">address</span></span>                | [<span data-ttu-id="59201-137">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="59201-137">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="59201-138">O endereço da sala ou da sala de salas.</span><span class="sxs-lookup"><span data-stu-id="59201-138">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="59201-139">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="59201-139">audioDeviceName</span></span>        | <span data-ttu-id="59201-140">String</span><span class="sxs-lookup"><span data-stu-id="59201-140">String</span></span>                                            | <span data-ttu-id="59201-141">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="59201-141">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="59201-142">bookingType</span><span class="sxs-lookup"><span data-stu-id="59201-142">bookingType</span></span>            | [<span data-ttu-id="59201-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="59201-143">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="59201-144">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="59201-144">Type of room.</span></span> <span data-ttu-id="59201-145">Os valores possíveis são: `Standard` e `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="59201-145">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="59201-146">Build</span><span class="sxs-lookup"><span data-stu-id="59201-146">building</span></span>               | <span data-ttu-id="59201-147">String</span><span class="sxs-lookup"><span data-stu-id="59201-147">String</span></span>                                            | <span data-ttu-id="59201-148">Especifica o nome do edifício ou o número de edifício em que a sala se encontra.</span><span class="sxs-lookup"><span data-stu-id="59201-148">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="59201-149">máxima</span><span class="sxs-lookup"><span data-stu-id="59201-149">capacity</span></span>               | <span data-ttu-id="59201-150">String</span><span class="sxs-lookup"><span data-stu-id="59201-150">String</span></span>                                            | <span data-ttu-id="59201-151">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="59201-151">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="59201-152">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="59201-152">displayDeviceName</span></span>      | <span data-ttu-id="59201-153">String</span><span class="sxs-lookup"><span data-stu-id="59201-153">String</span></span>                                            | <span data-ttu-id="59201-154">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="59201-154">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="59201-155">floorLabel</span><span class="sxs-lookup"><span data-stu-id="59201-155">floorLabel</span></span>             | <span data-ttu-id="59201-156">String</span><span class="sxs-lookup"><span data-stu-id="59201-156">String</span></span>                                            | <span data-ttu-id="59201-157">Especifica a carta de piso em que a sala está ativa.</span><span class="sxs-lookup"><span data-stu-id="59201-157">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="59201-158">floorNumber</span><span class="sxs-lookup"><span data-stu-id="59201-158">floorNumber</span></span>            | <span data-ttu-id="59201-159">Int32</span><span class="sxs-lookup"><span data-stu-id="59201-159">Int32</span></span>                                             | <span data-ttu-id="59201-160">Especifica o número do andar em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="59201-160">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="59201-161">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="59201-161">geoCoordinates</span></span>         | [<span data-ttu-id="59201-162">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="59201-162">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="59201-163">Especifica o local da sala ou da sala de opções no latitude, longitude e, opcionalmente, as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="59201-163">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="59201-164">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="59201-164">isWheelchairAccessible</span></span> | <span data-ttu-id="59201-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="59201-165">Boolean</span></span>                                           | <span data-ttu-id="59201-166">Especifica se a sala pode ser acessada por cadeira.</span><span class="sxs-lookup"><span data-stu-id="59201-166">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="59201-167">rótulo</span><span class="sxs-lookup"><span data-stu-id="59201-167">label</span></span>                  | <span data-ttu-id="59201-168">String</span><span class="sxs-lookup"><span data-stu-id="59201-168">String</span></span>                                            | <span data-ttu-id="59201-169">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="59201-169">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="59201-170">apelido</span><span class="sxs-lookup"><span data-stu-id="59201-170">nickname</span></span>               | <span data-ttu-id="59201-171">String</span><span class="sxs-lookup"><span data-stu-id="59201-171">String</span></span>                                            | <span data-ttu-id="59201-172">Especifica um apelido para a sala, por exemplo, "conf sala".</span><span class="sxs-lookup"><span data-stu-id="59201-172">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="59201-173">phone</span><span class="sxs-lookup"><span data-stu-id="59201-173">phone</span></span>                  | <span data-ttu-id="59201-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59201-174">String</span></span>                                            | <span data-ttu-id="59201-175">O número de telefone da sala ou sala de salas.</span><span class="sxs-lookup"><span data-stu-id="59201-175">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="59201-176">tags</span><span class="sxs-lookup"><span data-stu-id="59201-176">tags</span></span>                   | <span data-ttu-id="59201-177">Coleção String</span><span class="sxs-lookup"><span data-stu-id="59201-177">String collection</span></span>                                 | <span data-ttu-id="59201-178">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou tipo de mobília.</span><span class="sxs-lookup"><span data-stu-id="59201-178">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="59201-179">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="59201-179">videoDeviceName</span></span>        | <span data-ttu-id="59201-180">String</span><span class="sxs-lookup"><span data-stu-id="59201-180">String</span></span>                                            | <span data-ttu-id="59201-181">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="59201-181">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="59201-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="59201-182">Response</span></span>

<span data-ttu-id="59201-183">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Place](../resources/place.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59201-183">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59201-184">Exemplos</span><span class="sxs-lookup"><span data-stu-id="59201-184">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="59201-185">Exemplo 1: atualizar uma sala</span><span class="sxs-lookup"><span data-stu-id="59201-185">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="59201-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59201-186">Request</span></span>

<span data-ttu-id="59201-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59201-187">The following is an example of the request.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="59201-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="59201-188">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="59201-189">C#</span><span class="sxs-lookup"><span data-stu-id="59201-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59201-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59201-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59201-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59201-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59201-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="59201-192">Response</span></span>

<span data-ttu-id="59201-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59201-193">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="59201-194">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="59201-194">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59201-195">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59201-195">All the properties will be returned from an actual call.</span></span>

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
      "latitude": 47.0,
      "longitude": -122.0
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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="59201-196">Exemplo 2: atualizar uma salalist</span><span class="sxs-lookup"><span data-stu-id="59201-196">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="59201-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59201-197">Request</span></span>

<span data-ttu-id="59201-198">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59201-198">The following is an example of the request.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="59201-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="59201-199">HTTP</span></span>](#tab/http)
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
  "phone":"555-555-0100",
  "address": {
    "street": "4567 Main Street",
    "city": "Buffalo",
    "state": "NY",
    "postalCode": "98052",
    "countryOrRegion": "USA"
  },
  "geoCoordinates": {
    "altitude": null,
    "latitude": 47.0,
    "longitude": -122.0,
    "accuracy": null,
    "altitudeAccuracy": null
 }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59201-200">C#</span><span class="sxs-lookup"><span data-stu-id="59201-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59201-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59201-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59201-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59201-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59201-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="59201-203">Response</span></span>

<span data-ttu-id="59201-204">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59201-204">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="59201-205">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="59201-205">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59201-206">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59201-206">All the properties will be returned from an actual call.</span></span>

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
  "geoCoordinates": {
    "altitude": null,
    "latitude": 47.0,
    "longitude": -122.0,
    "accuracy": null,
    "altitudeAccuracy": null
 },
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
