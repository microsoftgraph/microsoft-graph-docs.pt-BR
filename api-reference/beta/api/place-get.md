---
title: Obter local
description: Recupere as propriedades e os relacionamentos de um objeto local.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a281c07e71d715ed123403fe16b2fd3fcc764a05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966909"
---
# <a name="get-place"></a><span data-ttu-id="9eff1-103">Obter local</span><span class="sxs-lookup"><span data-stu-id="9eff1-103">Get place</span></span>

<span data-ttu-id="9eff1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eff1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="9eff1-105">Obtenha as propriedades e os relacionamentos de um objeto [local](../resources/place.md) especificado por sua ID ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="9eff1-105">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="9eff1-106">O objeto **local** pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="9eff1-106">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="9eff1-107">Uma [sala](../resources/room.md) que inclui Propriedades sofisticadas, como um endereço de email para a sala, e suporte à acessibilidade, capacidade e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9eff1-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="9eff1-108">Uma [lista de salas](../resources/roomlist.md) que inclui um endereço de email para a lista de salas e uma propriedade de navegação para obter a coleção de instâncias de **sala** na lista de salas.</span><span class="sxs-lookup"><span data-stu-id="9eff1-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="9eff1-109">A **sala** e a **salalist** são derivadas do objeto [local](../resources/place.md) .</span><span class="sxs-lookup"><span data-stu-id="9eff1-109">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9eff1-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="9eff1-110">Permissions</span></span>

<span data-ttu-id="9eff1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9eff1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9eff1-113">Permission type</span></span>                        | <span data-ttu-id="9eff1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9eff1-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9eff1-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9eff1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="9eff1-116">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="9eff1-116">Place.Read.All</span></span> |
| <span data-ttu-id="9eff1-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9eff1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eff1-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9eff1-118">Not supported</span></span> |
| <span data-ttu-id="9eff1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9eff1-119">Application</span></span>                            | <span data-ttu-id="9eff1-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="9eff1-120">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eff1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9eff1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9eff1-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9eff1-122">Optional query parameters</span></span>
<span data-ttu-id="9eff1-123">Use $select para obter propriedades de **local** específico.</span><span class="sxs-lookup"><span data-stu-id="9eff1-123">Use $select to get specific **place** properties.</span></span>

<span data-ttu-id="9eff1-124">Para obter mais informações sobre opções de consulta OData, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9eff1-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9eff1-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9eff1-125">Request headers</span></span>

| <span data-ttu-id="9eff1-126">Nome</span><span class="sxs-lookup"><span data-stu-id="9eff1-126">Name</span></span>          | <span data-ttu-id="9eff1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eff1-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9eff1-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9eff1-128">Authorization</span></span> | <span data-ttu-id="9eff1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9eff1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9eff1-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9eff1-131">Request body</span></span>

<span data-ttu-id="9eff1-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9eff1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9eff1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eff1-133">Response</span></span>

<span data-ttu-id="9eff1-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [local](../resources/place.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9eff1-134">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9eff1-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9eff1-135">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="9eff1-136">Exemplo 1: obter uma sala</span><span class="sxs-lookup"><span data-stu-id="9eff1-136">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="9eff1-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9eff1-137">Request</span></span>

<span data-ttu-id="9eff1-138">O exemplo a seguir especifica a **ID** de uma **sala** para obter suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9eff1-138">The following example specifies the **id** of a **room** to get its properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="9eff1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9eff1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="c"></a>[<span data-ttu-id="9eff1-140">C#</span><span class="sxs-lookup"><span data-stu-id="9eff1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9eff1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9eff1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9eff1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9eff1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9eff1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eff1-143">Response</span></span>

<span data-ttu-id="9eff1-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9eff1-144">The following is an example of the response.</span></span>

><span data-ttu-id="9eff1-145">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9eff1-145">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9eff1-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9eff1-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_room",
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
    "phone": "000-000-0000",
    "nickname": "Conf Room",
    "label": "100",
    "capacity": "50",
    "building": "1",
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

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="9eff1-147">Exemplo 2: obter uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="9eff1-147">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="9eff1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9eff1-148">Request</span></span>

<span data-ttu-id="9eff1-149">O exemplo a seguir especifica o **EmailAddress** de uma **RoomList** para obter suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9eff1-149">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="9eff1-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="9eff1-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```
# <a name="c"></a>[<span data-ttu-id="9eff1-151">C#</span><span class="sxs-lookup"><span data-stu-id="9eff1-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9eff1-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9eff1-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9eff1-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9eff1-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9eff1-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eff1-154">Response</span></span>

<span data-ttu-id="9eff1-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9eff1-155">The following is an example of the response.</span></span>

><span data-ttu-id="9eff1-156">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9eff1-156">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9eff1-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9eff1-157">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roomlist",
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
  "phone": null,
  "emailAddress": "bldg1@contoso.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


