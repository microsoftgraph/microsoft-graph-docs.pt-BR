---
title: Local de atualização
description: Atualize as propriedades do objeto local.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: bb803037298c34f6c3410bf57e9f7ed180431066
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904530"
---
# <a name="update-place"></a><span data-ttu-id="d81a1-103">Local de atualização</span><span class="sxs-lookup"><span data-stu-id="d81a1-103">Update place</span></span>

<span data-ttu-id="d81a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d81a1-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d81a1-105">Atualize as propriedades do objeto [local](../resources/place.md) , que pode ser uma [sala](../resources/room.md) ou uma [sala de salas](../resources/roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="d81a1-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="d81a1-106">Você pode identificar a **sala** ou a **sala de salas** especificando a propriedade **ID** ou **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="d81a1-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="d81a1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d81a1-107">Permissions</span></span>

<span data-ttu-id="d81a1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d81a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d81a1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d81a1-110">Permission type</span></span>                        | <span data-ttu-id="d81a1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d81a1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d81a1-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d81a1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d81a1-113">Place.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81a1-113">Place.ReadWrite.All</span></span> |
| <span data-ttu-id="d81a1-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d81a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d81a1-115">Not supported.</span></span> |
| <span data-ttu-id="d81a1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d81a1-116">Application</span></span>                            | <span data-ttu-id="d81a1-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d81a1-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="d81a1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d81a1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="d81a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d81a1-119">Request headers</span></span>

| <span data-ttu-id="d81a1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d81a1-120">Name</span></span>       | <span data-ttu-id="d81a1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d81a1-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d81a1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d81a1-122">Authorization</span></span>  | <span data-ttu-id="d81a1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d81a1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d81a1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d81a1-125">Content-Type</span></span> | <span data-ttu-id="d81a1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d81a1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d81a1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d81a1-128">Request body</span></span>

<span data-ttu-id="d81a1-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d81a1-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d81a1-130">Somente uma instância de um recurso de colocar ( **sala** ou **sala de salas** ) pode ser atualizada de cada vez.</span><span class="sxs-lookup"><span data-stu-id="d81a1-130">Only one instance of a place resource ( **room** or **roomList** ) can be updated at a time.</span></span> <span data-ttu-id="d81a1-131">No corpo da solicitação, use `@odata.type` para especificar o tipo de local e inclua as propriedades desse tipo para atualizar.</span><span class="sxs-lookup"><span data-stu-id="d81a1-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="d81a1-132">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d81a1-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d81a1-133">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d81a1-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d81a1-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d81a1-134">Property</span></span>               | <span data-ttu-id="d81a1-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d81a1-135">Type</span></span>                                              | <span data-ttu-id="d81a1-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d81a1-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="d81a1-137">address</span><span class="sxs-lookup"><span data-stu-id="d81a1-137">address</span></span>                | [<span data-ttu-id="d81a1-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d81a1-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="d81a1-139">O endereço da sala ou da sala de salas.</span><span class="sxs-lookup"><span data-stu-id="d81a1-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="d81a1-140">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="d81a1-140">audioDeviceName</span></span>        | <span data-ttu-id="d81a1-141">String</span><span class="sxs-lookup"><span data-stu-id="d81a1-141">String</span></span>                                            | <span data-ttu-id="d81a1-142">Especifica o nome do dispositivo de áudio na sala.</span><span class="sxs-lookup"><span data-stu-id="d81a1-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="d81a1-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="d81a1-143">bookingType</span></span>            | [<span data-ttu-id="d81a1-144">bookingType</span><span class="sxs-lookup"><span data-stu-id="d81a1-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="d81a1-145">Tipo de sala.</span><span class="sxs-lookup"><span data-stu-id="d81a1-145">Type of room.</span></span> <span data-ttu-id="d81a1-146">Os valores possíveis são: `Standard` e `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="d81a1-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="d81a1-147">Build</span><span class="sxs-lookup"><span data-stu-id="d81a1-147">building</span></span>               | <span data-ttu-id="d81a1-148">String</span><span class="sxs-lookup"><span data-stu-id="d81a1-148">String</span></span>                                            | <span data-ttu-id="d81a1-149">Especifica o nome do edifício ou o número de edifício em que a sala se encontra.</span><span class="sxs-lookup"><span data-stu-id="d81a1-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="d81a1-150">máxima</span><span class="sxs-lookup"><span data-stu-id="d81a1-150">capacity</span></span>               | <span data-ttu-id="d81a1-151">String</span><span class="sxs-lookup"><span data-stu-id="d81a1-151">String</span></span>                                            | <span data-ttu-id="d81a1-152">Especifica a capacidade da sala.</span><span class="sxs-lookup"><span data-stu-id="d81a1-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="d81a1-153">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="d81a1-153">displayDeviceName</span></span>      | <span data-ttu-id="d81a1-154">String</span><span class="sxs-lookup"><span data-stu-id="d81a1-154">String</span></span>                                            | <span data-ttu-id="d81a1-155">Especifica o nome do dispositivo de exibição na sala.</span><span class="sxs-lookup"><span data-stu-id="d81a1-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="d81a1-156">floorLabel</span><span class="sxs-lookup"><span data-stu-id="d81a1-156">floorLabel</span></span>             | <span data-ttu-id="d81a1-157">String</span><span class="sxs-lookup"><span data-stu-id="d81a1-157">String</span></span>                                            | <span data-ttu-id="d81a1-158">Especifica a carta de piso em que a sala está ativa.</span><span class="sxs-lookup"><span data-stu-id="d81a1-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="d81a1-159">floorNumber</span><span class="sxs-lookup"><span data-stu-id="d81a1-159">floorNumber</span></span>            | <span data-ttu-id="d81a1-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d81a1-160">Int32</span></span>                                             | <span data-ttu-id="d81a1-161">Especifica o número do andar em que a sala está.</span><span class="sxs-lookup"><span data-stu-id="d81a1-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="d81a1-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d81a1-162">geoCoordinates</span></span>         | [<span data-ttu-id="d81a1-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d81a1-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="d81a1-164">Especifica o local da sala ou da sala de opções no latitude, longitude e, opcionalmente, as coordenadas de altitude.</span><span class="sxs-lookup"><span data-stu-id="d81a1-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="d81a1-165">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="d81a1-165">isWheelchairAccessible</span></span> | <span data-ttu-id="d81a1-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="d81a1-166">Boolean</span></span>                                           | <span data-ttu-id="d81a1-167">Especifica se a sala pode ser acessada por cadeira.</span><span class="sxs-lookup"><span data-stu-id="d81a1-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="d81a1-168">rótulo</span><span class="sxs-lookup"><span data-stu-id="d81a1-168">label</span></span>                  | <span data-ttu-id="d81a1-169">String</span><span class="sxs-lookup"><span data-stu-id="d81a1-169">String</span></span>                                            | <span data-ttu-id="d81a1-170">Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome.</span><span class="sxs-lookup"><span data-stu-id="d81a1-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="d81a1-171">apelido</span><span class="sxs-lookup"><span data-stu-id="d81a1-171">nickname</span></span>               | <span data-ttu-id="d81a1-172">String</span><span class="sxs-lookup"><span data-stu-id="d81a1-172">String</span></span>                                            | <span data-ttu-id="d81a1-173">Especifica um apelido para a sala, por exemplo, "conf sala".</span><span class="sxs-lookup"><span data-stu-id="d81a1-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="d81a1-174">phone</span><span class="sxs-lookup"><span data-stu-id="d81a1-174">phone</span></span>                  | <span data-ttu-id="d81a1-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d81a1-175">String</span></span>                                            | <span data-ttu-id="d81a1-176">O número de telefone da sala ou sala de salas.</span><span class="sxs-lookup"><span data-stu-id="d81a1-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="d81a1-177">categorias</span><span class="sxs-lookup"><span data-stu-id="d81a1-177">tags</span></span>                   | <span data-ttu-id="d81a1-178">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d81a1-178">String collection</span></span>                                 | <span data-ttu-id="d81a1-179">Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou tipo de mobília.</span><span class="sxs-lookup"><span data-stu-id="d81a1-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="d81a1-180">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="d81a1-180">videoDeviceName</span></span>        | <span data-ttu-id="d81a1-181">String</span><span class="sxs-lookup"><span data-stu-id="d81a1-181">String</span></span>                                            | <span data-ttu-id="d81a1-182">Especifica o nome do dispositivo de vídeo na sala.</span><span class="sxs-lookup"><span data-stu-id="d81a1-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="d81a1-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81a1-183">Response</span></span>

<span data-ttu-id="d81a1-184">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Place](../resources/place.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d81a1-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d81a1-185">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d81a1-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="d81a1-186">Exemplo 1: atualizar uma sala</span><span class="sxs-lookup"><span data-stu-id="d81a1-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="d81a1-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d81a1-187">Request</span></span>

<span data-ttu-id="d81a1-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d81a1-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="d81a1-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81a1-189">HTTP</span></span>](#tab/http)
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
  "capacity": "50",
  "isWheelchairAccessible": false
}
```
# <a name="c"></a>[<span data-ttu-id="d81a1-190">C#</span><span class="sxs-lookup"><span data-stu-id="d81a1-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d81a1-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81a1-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d81a1-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81a1-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d81a1-193">Java</span><span class="sxs-lookup"><span data-stu-id="d81a1-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d81a1-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81a1-194">Response</span></span>

<span data-ttu-id="d81a1-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d81a1-195">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d81a1-196">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d81a1-196">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d81a1-197">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d81a1-197">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="d81a1-198">Exemplo 2: atualizar uma salalist</span><span class="sxs-lookup"><span data-stu-id="d81a1-198">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="d81a1-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d81a1-199">Request</span></span>

<span data-ttu-id="d81a1-200">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d81a1-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d81a1-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81a1-201">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d81a1-202">C#</span><span class="sxs-lookup"><span data-stu-id="d81a1-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d81a1-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81a1-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d81a1-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81a1-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d81a1-205">Java</span><span class="sxs-lookup"><span data-stu-id="d81a1-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d81a1-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81a1-206">Response</span></span>

<span data-ttu-id="d81a1-207">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d81a1-207">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d81a1-208">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d81a1-208">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d81a1-209">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d81a1-209">All the properties will be returned from an actual call.</span></span>

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

