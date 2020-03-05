---
title: Locais de lista
description: Recupere uma lista de objetos Place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ee17676564f747064e08066c830e7ebc21d36805
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455820"
---
# <a name="list-places"></a><span data-ttu-id="95966-103">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="95966-103">List places</span></span>

<span data-ttu-id="95966-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95966-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95966-105">Obtém uma coleção do tipo especificado de objetos [Place](../resources/place.md) definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="95966-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="95966-106">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="95966-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="95966-107">Um objeto **local** pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="95966-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="95966-108">Uma [sala](../resources/room.md) que inclui Propriedades sofisticadas, como um endereço de email para a sala, e suporte à acessibilidade, capacidade e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95966-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="95966-109">Uma [lista de salas](../resources/roomlist.md) que inclui um endereço de email para a lista de salas e uma propriedade de navegação para obter a coleção de instâncias de sala na lista de salas.</span><span class="sxs-lookup"><span data-stu-id="95966-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="95966-110">A **sala** e a **salalist** são derivadas do objeto **local** .</span><span class="sxs-lookup"><span data-stu-id="95966-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="95966-111">Em comparação com as funções [findRooms](../api/user-findrooms.md) e [findRoomLists](../api/user-findroomlists.md) , essa operação retorna uma carga mais rica para salas e listas de salas.</span><span class="sxs-lookup"><span data-stu-id="95966-111">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="95966-112">Veja [detalhes](../resources/place.md#using-the-places-api) sobre como eles se comparam.</span><span class="sxs-lookup"><span data-stu-id="95966-112">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="95966-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="95966-113">Permissions</span></span>

<span data-ttu-id="95966-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95966-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95966-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95966-116">Permission type</span></span>                        | <span data-ttu-id="95966-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95966-117">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="95966-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95966-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="95966-119">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="95966-119">Place.Read.All</span></span> |
| <span data-ttu-id="95966-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95966-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95966-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="95966-121">Not supported</span></span> |
| <span data-ttu-id="95966-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95966-122">Application</span></span>                            | <span data-ttu-id="95966-123">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="95966-123">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95966-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95966-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="95966-125">Para obter todas as salas em um locatário:</span><span class="sxs-lookup"><span data-stu-id="95966-125">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="95966-126">Para obter todas as listas de salas em um locatário:</span><span class="sxs-lookup"><span data-stu-id="95966-126">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="95966-127">Para obter todas as salas na lista de salas especificada:</span><span class="sxs-lookup"><span data-stu-id="95966-127">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="95966-128">**Observação**: para obter salas em uma lista de salas, você deve especificar a lista de salas por sua propriedade **EmailAddress** , não pela **ID**.</span><span class="sxs-lookup"><span data-stu-id="95966-128">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="95966-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="95966-129">Optional query parameters</span></span>

<span data-ttu-id="95966-130">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="95966-130">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="95966-131">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="95966-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="95966-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95966-132">Request headers</span></span>

| <span data-ttu-id="95966-133">Nome</span><span class="sxs-lookup"><span data-stu-id="95966-133">Name</span></span>          | <span data-ttu-id="95966-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="95966-134">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="95966-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="95966-135">Authorization</span></span> | <span data-ttu-id="95966-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95966-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95966-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95966-138">Request body</span></span>

<span data-ttu-id="95966-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95966-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95966-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="95966-140">Response</span></span>

<span data-ttu-id="95966-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de [colocar](../resources/place.md) objetos no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95966-141">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95966-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="95966-142">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="95966-143">Exemplo 1: listar todas as salas definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="95966-143">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="95966-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95966-144">Request</span></span>

<span data-ttu-id="95966-145">O exemplo a seguir mostra como obter todos os objetos de [sala](../resources/room.md) no locatário.</span><span class="sxs-lookup"><span data-stu-id="95966-145">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="95966-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="95966-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```
# <a name="c"></a>[<span data-ttu-id="95966-147">C#</span><span class="sxs-lookup"><span data-stu-id="95966-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95966-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95966-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95966-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95966-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95966-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="95966-150">Response</span></span>

<span data-ttu-id="95966-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95966-151">The following is an example of the response.</span></span>

><span data-ttu-id="95966-152">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="95966-152">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95966-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95966-153">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="95966-154">Exemplo 2: listar todas as listas de salas definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="95966-154">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="95966-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95966-155">Request</span></span>

<span data-ttu-id="95966-156">O exemplo a seguir mostra como obter todos os objetos [RoomList](../resources/roomlist.md) no locatário.</span><span class="sxs-lookup"><span data-stu-id="95966-156">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="95966-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="95966-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```
# <a name="c"></a>[<span data-ttu-id="95966-158">C#</span><span class="sxs-lookup"><span data-stu-id="95966-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95966-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95966-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95966-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95966-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95966-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="95966-161">Response</span></span>

<span data-ttu-id="95966-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95966-162">The following is an example of the response.</span></span>

><span data-ttu-id="95966-163">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="95966-163">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95966-164">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95966-164">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="95966-165">Exemplo 3: listar salas contidas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="95966-165">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="95966-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95966-166">Request</span></span>

<span data-ttu-id="95966-167">O exemplo a seguir mostra como obter uma lista de objetos [Room](../resources/room.md) contidos em uma **salalist**.</span><span class="sxs-lookup"><span data-stu-id="95966-167">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="95966-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="95966-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="c"></a>[<span data-ttu-id="95966-169">C#</span><span class="sxs-lookup"><span data-stu-id="95966-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95966-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95966-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95966-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95966-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95966-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="95966-172">Response</span></span>

<span data-ttu-id="95966-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95966-173">The following is an example of the response.</span></span>

><span data-ttu-id="95966-174">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="95966-174">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95966-175">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95966-175">All the properties will be returned from an actual call.</span></span>

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
