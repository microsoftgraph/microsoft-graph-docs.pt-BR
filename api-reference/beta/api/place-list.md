---
title: Locais de lista
description: Recupere uma lista de objetos Place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1dddab1015265b5eb26ccdd0824c25684ee3421a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413605"
---
# <a name="list-places"></a><span data-ttu-id="7ae00-103">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="7ae00-103">List places</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ae00-104">Obtém uma coleção do tipo especificado de objetos [Place](../resources/place.md) definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="7ae00-104">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="7ae00-105">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="7ae00-105">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="7ae00-106">Um objeto **local** pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="7ae00-106">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="7ae00-107">Uma [sala](../resources/room.md) que inclui Propriedades sofisticadas, como um endereço de email para a sala, e suporte à acessibilidade, capacidade e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ae00-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="7ae00-108">Uma [lista de salas](../resources/roomlist.md) que inclui um endereço de email para a lista de salas e uma propriedade de navegação para obter a coleção de instâncias de sala na lista de salas.</span><span class="sxs-lookup"><span data-stu-id="7ae00-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="7ae00-109">A **sala** e \*\*\*\* a salalist são derivadas do objeto **local** .</span><span class="sxs-lookup"><span data-stu-id="7ae00-109">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="7ae00-110">Em comparação com as funções [findRooms](../api/user-findrooms.md) e [findRoomLists](../api/user-findroomlists.md) , essa operação retorna uma carga mais rica para salas e listas de salas.</span><span class="sxs-lookup"><span data-stu-id="7ae00-110">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="7ae00-111">Veja [detalhes](../resources/place.md#using-the-places-api) sobre como eles se comparam.</span><span class="sxs-lookup"><span data-stu-id="7ae00-111">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ae00-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ae00-112">Permissions</span></span>

<span data-ttu-id="7ae00-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ae00-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ae00-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ae00-115">Permission type</span></span>                        | <span data-ttu-id="7ae00-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ae00-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7ae00-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ae00-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ae00-118">Local. Read. All</span><span class="sxs-lookup"><span data-stu-id="7ae00-118">Place.Read.All</span></span> |
| <span data-ttu-id="7ae00-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ae00-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ae00-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7ae00-120">Not supported</span></span> |
| <span data-ttu-id="7ae00-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ae00-121">Application</span></span>                            | <span data-ttu-id="7ae00-122">Local. Read. All</span><span class="sxs-lookup"><span data-stu-id="7ae00-122">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ae00-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ae00-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="7ae00-124">Para obter todas as salas em um locatário:</span><span class="sxs-lookup"><span data-stu-id="7ae00-124">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="7ae00-125">Para obter todas as listas de salas em um locatário:</span><span class="sxs-lookup"><span data-stu-id="7ae00-125">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="7ae00-126">Para obter todas as salas na lista de salas especificada:</span><span class="sxs-lookup"><span data-stu-id="7ae00-126">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="7ae00-127">**Observação**: para obter salas em uma lista de salas, você deve especificar a lista de salas por sua propriedade **EmailAddress** , não pela **ID**.</span><span class="sxs-lookup"><span data-stu-id="7ae00-127">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="7ae00-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ae00-128">Optional query parameters</span></span>

<span data-ttu-id="7ae00-129">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ae00-129">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7ae00-130">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7ae00-130">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ae00-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae00-131">Request headers</span></span>

| <span data-ttu-id="7ae00-132">Nome</span><span class="sxs-lookup"><span data-stu-id="7ae00-132">Name</span></span>          | <span data-ttu-id="7ae00-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ae00-133">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7ae00-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ae00-134">Authorization</span></span> | <span data-ttu-id="7ae00-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ae00-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ae00-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae00-137">Request body</span></span>

<span data-ttu-id="7ae00-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ae00-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ae00-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ae00-139">Response</span></span>

<span data-ttu-id="7ae00-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de [colocar](../resources/place.md) objetos no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ae00-140">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ae00-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7ae00-141">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="7ae00-142">Exemplo 1: listar todas as salas definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="7ae00-142">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="7ae00-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae00-143">Request</span></span>

<span data-ttu-id="7ae00-144">O exemplo a seguir mostra como obter todos os objetos de [sala](../resources/room.md) no locatário.</span><span class="sxs-lookup"><span data-stu-id="7ae00-144">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7ae00-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ae00-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ae00-146">C#</span><span class="sxs-lookup"><span data-stu-id="7ae00-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ae00-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ae00-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ae00-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7ae00-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ae00-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ae00-149">Response</span></span>

<span data-ttu-id="7ae00-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ae00-150">The following is an example of the response.</span></span>

><span data-ttu-id="7ae00-151">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ae00-151">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ae00-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ae00-152">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_all_rooms",
  "truncated": true,
  "@odata.type": "microsoft.graph.room",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/microsoft.graph.room",
  "value": [
    {
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
    },
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78970B97",
      "emailAddress": "cf200@contoso.com",
      "displayName": "Conf Room 200",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488625,
        "longitude": -122.1293731033802
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "200",
      "capacity": "40",
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelchairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "benches",
        "nice view"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    }
  ]
}
```

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="7ae00-153">Exemplo 2: listar todas as listas de salas definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="7ae00-153">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="7ae00-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae00-154">Request</span></span>

<span data-ttu-id="7ae00-155">O exemplo a seguir mostra como obter todos os [](../resources/roomlist.md) objetos RoomList no locatário.</span><span class="sxs-lookup"><span data-stu-id="7ae00-155">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7ae00-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ae00-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ae00-157">C#</span><span class="sxs-lookup"><span data-stu-id="7ae00-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ae00-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ae00-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ae00-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7ae00-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ae00-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ae00-160">Response</span></span>

<span data-ttu-id="7ae00-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ae00-161">The following is an example of the response.</span></span>

><span data-ttu-id="7ae00-162">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ae00-162">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ae00-163">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ae00-163">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_all_roomlists",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/microsoft.graph.roomList",
  "value": [
    {
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
    },
    {
      "id": "DC404124-302A-92AA-F98D-7B4DEB0C1706",
      "displayName": "Building 2",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geocoordinates": null,
      "phone": null,
      "emailAddress": "bldg2@contoso.com"
    }
  ]
}
```

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="7ae00-164">Exemplo 3: listar salas contidas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="7ae00-164">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="7ae00-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ae00-165">Request</span></span>

<span data-ttu-id="7ae00-166">O exemplo a seguir mostra como obter uma lista de objetos [Room](../resources/room.md) contidos em uma **salalist**.</span><span class="sxs-lookup"><span data-stu-id="7ae00-166">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="7ae00-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ae00-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ae00-168">C#</span><span class="sxs-lookup"><span data-stu-id="7ae00-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ae00-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ae00-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ae00-170">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7ae00-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ae00-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ae00-171">Response</span></span>

<span data-ttu-id="7ae00-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ae00-172">The following is an example of the response.</span></span>

><span data-ttu-id="7ae00-173">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ae00-173">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ae00-174">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ae00-174">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_rooms_in_roomlist",
  "truncated": true,
  "@odata.type": "microsoft.graph.room",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places('bldg2%40contoso.com')/microsoft.graph.roomList/rooms",
  "value": [
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78970B97",
      "emailAddress": "cf200@contoso.com",
      "displayName": "Conf Room 200",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488625,
        "longitude": -122.1293731033802
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "200",
      "capacity": "40",
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelchairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "benches",
        "nice view"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List places",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: Malformed function params 'id-of-roomlist'"
  ]
}-->
