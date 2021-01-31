---
title: Local de atualização
description: Atualize as propriedades do objeto place.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 3ce93b0d170c0aca27c6814d319a2161cacc1050
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059613"
---
# <a name="update-place"></a><span data-ttu-id="df687-103">Local de atualização</span><span class="sxs-lookup"><span data-stu-id="df687-103">Update place</span></span>

<span data-ttu-id="df687-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df687-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="df687-105">Atualizar as propriedades do [objeto place,](../resources/place.md) que pode ser uma [sala](../resources/room.md) ou [roomList](../resources/roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="df687-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="df687-106">Você pode identificar a **sala ou** **roomList** especificando a **id** ou **a propriedade emailAddress.**</span><span class="sxs-lookup"><span data-stu-id="df687-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="df687-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="df687-107">Permissions</span></span>

<span data-ttu-id="df687-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df687-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df687-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df687-110">Permission type</span></span>                        | <span data-ttu-id="df687-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df687-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df687-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df687-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="df687-113">Place.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df687-113">Place.ReadWrite.All</span></span> |
| <span data-ttu-id="df687-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df687-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df687-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df687-115">Not supported.</span></span> |
| <span data-ttu-id="df687-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df687-116">Application</span></span>                            | <span data-ttu-id="df687-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="df687-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="df687-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df687-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="df687-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df687-119">Request headers</span></span>

| <span data-ttu-id="df687-120">Nome</span><span class="sxs-lookup"><span data-stu-id="df687-120">Name</span></span>       | <span data-ttu-id="df687-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df687-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="df687-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df687-122">Authorization</span></span>  | <span data-ttu-id="df687-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df687-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df687-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df687-125">Content-Type</span></span> | <span data-ttu-id="df687-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df687-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df687-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df687-128">Request body</span></span>

<span data-ttu-id="df687-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="df687-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="df687-130">Apenas uma instância de um recurso de local **(sala** ou **roomList**) pode ser atualizada por vez.</span><span class="sxs-lookup"><span data-stu-id="df687-130">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="df687-131">No corpo da solicitação, use para especificar o tipo de local e incluir as `@odata.type` propriedades desse tipo a atualizar.</span><span class="sxs-lookup"><span data-stu-id="df687-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="df687-132">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="df687-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="df687-133">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="df687-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="df687-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df687-134">Property</span></span>               | <span data-ttu-id="df687-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="df687-135">Type</span></span>                                              | <span data-ttu-id="df687-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="df687-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="df687-137">address</span><span class="sxs-lookup"><span data-stu-id="df687-137">address</span></span>                | [<span data-ttu-id="df687-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="df687-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="df687-139">O endereço da sala ou da lista de sala.</span><span class="sxs-lookup"><span data-stu-id="df687-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="df687-140">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="df687-140">audioDeviceName</span></span>        | <span data-ttu-id="df687-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-141">String</span></span>                                            | <span data-ttu-id="df687-142">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="df687-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="df687-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="df687-143">bookingType</span></span>            | [<span data-ttu-id="df687-144">bookingType</span><span class="sxs-lookup"><span data-stu-id="df687-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="df687-145">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="df687-145">Type of room.</span></span> <span data-ttu-id="df687-146">Os valores possíveis são: `Standard` e `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="df687-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="df687-147">building</span><span class="sxs-lookup"><span data-stu-id="df687-147">building</span></span>               | <span data-ttu-id="df687-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-148">String</span></span>                                            | <span data-ttu-id="df687-149">Especifica o nome do edifício ou o número do edifício em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="df687-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="df687-150">capacity</span><span class="sxs-lookup"><span data-stu-id="df687-150">capacity</span></span>               | <span data-ttu-id="df687-151">Int32</span><span class="sxs-lookup"><span data-stu-id="df687-151">Int32</span></span>                                             | <span data-ttu-id="df687-152">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="df687-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="df687-153">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="df687-153">displayDeviceName</span></span>      | <span data-ttu-id="df687-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-154">String</span></span>                                            | <span data-ttu-id="df687-155">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="df687-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="df687-156">floorLabel</span><span class="sxs-lookup"><span data-stu-id="df687-156">floorLabel</span></span>             | <span data-ttu-id="df687-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-157">String</span></span>                                            | <span data-ttu-id="df687-158">Especifica a letra do piso em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="df687-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="df687-159">floorNumber</span><span class="sxs-lookup"><span data-stu-id="df687-159">floorNumber</span></span>            | <span data-ttu-id="df687-160">Int32</span><span class="sxs-lookup"><span data-stu-id="df687-160">Int32</span></span>                                             | <span data-ttu-id="df687-161">Especifica o número do piso em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="df687-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="df687-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="df687-162">geoCoordinates</span></span>         | [<span data-ttu-id="df687-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="df687-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="df687-164">Especifica o local da sala ou da lista de sala em coordenadas de latitude, longitude e, opcionalmente, altitude.</span><span class="sxs-lookup"><span data-stu-id="df687-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="df687-165">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="df687-165">isWheelChairAccessible</span></span> | <span data-ttu-id="df687-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="df687-166">Boolean</span></span>                                           | <span data-ttu-id="df687-167">Especifica se a sala é acessível para acessibilidade.</span><span class="sxs-lookup"><span data-stu-id="df687-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="df687-168">rótulo</span><span class="sxs-lookup"><span data-stu-id="df687-168">label</span></span>                  | <span data-ttu-id="df687-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-169">String</span></span>                                            | <span data-ttu-id="df687-170">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="df687-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="df687-171">nickname</span><span class="sxs-lookup"><span data-stu-id="df687-171">nickname</span></span>               | <span data-ttu-id="df687-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-172">String</span></span>                                            | <span data-ttu-id="df687-173">Especifica um apelido para a sala, por exemplo, "conf room".</span><span class="sxs-lookup"><span data-stu-id="df687-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="df687-174">phone</span><span class="sxs-lookup"><span data-stu-id="df687-174">phone</span></span>                  | <span data-ttu-id="df687-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-175">String</span></span>                                            | <span data-ttu-id="df687-176">O número de telefone da sala ou da lista de sala.</span><span class="sxs-lookup"><span data-stu-id="df687-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="df687-177">tags</span><span class="sxs-lookup"><span data-stu-id="df687-177">tags</span></span>                   | <span data-ttu-id="df687-178">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-178">String collection</span></span>                                 | <span data-ttu-id="df687-179">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou o tipo de móveis.</span><span class="sxs-lookup"><span data-stu-id="df687-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="df687-180">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="df687-180">videoDeviceName</span></span>        | <span data-ttu-id="df687-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df687-181">String</span></span>                                            | <span data-ttu-id="df687-182">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="df687-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="df687-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="df687-183">Response</span></span>

<span data-ttu-id="df687-184">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [place](../resources/place.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df687-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df687-185">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df687-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="df687-186">Exemplo 1: Atualizar uma sala</span><span class="sxs-lookup"><span data-stu-id="df687-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="df687-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df687-187">Request</span></span>

<span data-ttu-id="df687-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df687-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="df687-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="df687-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_room"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/cf100@contoso.com
Content-type: application/json
Content-length: 285

{
  "@odata.type": "microsoft.graph.room",
  "nickname": "Conf Room",
  "building": "1",
  "label": "100",
  "capacity": 50,
  "isWheelChairAccessible": false
}
```
# <a name="c"></a>[<span data-ttu-id="df687-190">C#</span><span class="sxs-lookup"><span data-stu-id="df687-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df687-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df687-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df687-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df687-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df687-193">Java</span><span class="sxs-lookup"><span data-stu-id="df687-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df687-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="df687-194">Response</span></span>

<span data-ttu-id="df687-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df687-195">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="df687-196">O objeto response mostrado aqui pode ser encurtado para maior leitura.</span><span class="sxs-lookup"><span data-stu-id="df687-196">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="df687-197">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df687-197">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/$entity",
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
    "capacity": 50,
    "building": "1",
    "floorLabel": "1P",
    "floorNumber": 1,
    "isManaged": true,
    "isWheelChairAccessible": false,
    "bookingType": "standard",
    "tags": [
      "bean bags"
    ],
    "audioDeviceName": null,
    "videoDeviceName": null,
    "displayDevice": "surface hub"
}
```

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="df687-198">Exemplo 2: Atualizar uma lista de sala</span><span class="sxs-lookup"><span data-stu-id="df687-198">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="df687-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df687-199">Request</span></span>

<span data-ttu-id="df687-200">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df687-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="df687-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="df687-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/Building1RroomList@contoso.onmicrosoft.com
Content-type: application/json

{
  "@odata.type": "microsoft.graph.roomList",
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
# <a name="c"></a>[<span data-ttu-id="df687-202">C#</span><span class="sxs-lookup"><span data-stu-id="df687-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df687-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df687-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df687-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df687-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df687-205">Java</span><span class="sxs-lookup"><span data-stu-id="df687-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="df687-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="df687-206">Response</span></span>

<span data-ttu-id="df687-207">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df687-207">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="df687-208">O objeto response mostrado aqui pode ser encurtado para maior leitura.</span><span class="sxs-lookup"><span data-stu-id="df687-208">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="df687-209">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df687-209">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/$entity",
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

