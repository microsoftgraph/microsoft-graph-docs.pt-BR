---
title: Locais de lista
description: Recupere uma lista de objetos Place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 27835ec7eea8c1bd40fd07be41900171465da3e2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876732"
---
# <a name="list-places"></a><span data-ttu-id="c33aa-103">Locais de lista</span><span class="sxs-lookup"><span data-stu-id="c33aa-103">List places</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c33aa-104">Obtém uma coleção do tipo especificado de objetos [Place](../resources/place.md) definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="c33aa-104">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="c33aa-105">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="c33aa-105">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="c33aa-106">Um objeto **local** pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="c33aa-106">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="c33aa-107">Uma [sala](../resources/room.md) que inclui Propriedades sofisticadas, como um endereço de email para a sala, e suporte à acessibilidade, capacidade e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c33aa-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="c33aa-108">Uma [lista de salas](../resources/roomlist.md) que inclui um endereço de email para a lista de salas e uma propriedade de navegação para obter a coleção de instâncias de sala na lista de salas.</span><span class="sxs-lookup"><span data-stu-id="c33aa-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="c33aa-109">A **sala** e \*\*\*\* a salalist são derivadas do objeto **local** .</span><span class="sxs-lookup"><span data-stu-id="c33aa-109">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="c33aa-110">Em comparação com as funções [findRooms](../api/user-findrooms.md) e [findRoomLists](../api/user-findroomlists.md) , essa operação retorna uma carga mais rica para salas e listas de salas.</span><span class="sxs-lookup"><span data-stu-id="c33aa-110">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="c33aa-111">Veja [detalhes](../resources/place.md#using-the-places-api) sobre como eles se comparam.</span><span class="sxs-lookup"><span data-stu-id="c33aa-111">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="c33aa-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="c33aa-112">Permissions</span></span>

<span data-ttu-id="c33aa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c33aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c33aa-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c33aa-115">Permission type</span></span>                        | <span data-ttu-id="c33aa-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c33aa-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c33aa-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c33aa-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="c33aa-118">Local. Read. All</span><span class="sxs-lookup"><span data-stu-id="c33aa-118">Place.Read.All</span></span> |
| <span data-ttu-id="c33aa-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c33aa-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c33aa-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c33aa-120">Not supported</span></span> |
| <span data-ttu-id="c33aa-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c33aa-121">Application</span></span>                            | <span data-ttu-id="c33aa-122">Local. Read. All</span><span class="sxs-lookup"><span data-stu-id="c33aa-122">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c33aa-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c33aa-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="c33aa-124">Para obter todas as salas em um locatário:</span><span class="sxs-lookup"><span data-stu-id="c33aa-124">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="c33aa-125">Para obter todas as listas de salas em um locatário:</span><span class="sxs-lookup"><span data-stu-id="c33aa-125">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="c33aa-126">Para obter todas as salas na lista de salas especificada:</span><span class="sxs-lookup"><span data-stu-id="c33aa-126">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="c33aa-127">**Observação**: para obter salas em uma lista de salas, você deve especificar a lista de salas por sua propriedade **EmailAddress** , não pela **ID**.</span><span class="sxs-lookup"><span data-stu-id="c33aa-127">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="c33aa-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c33aa-128">Optional query parameters</span></span>

<span data-ttu-id="c33aa-129">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c33aa-129">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c33aa-130">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c33aa-130">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c33aa-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c33aa-131">Request headers</span></span>

| <span data-ttu-id="c33aa-132">Nome</span><span class="sxs-lookup"><span data-stu-id="c33aa-132">Name</span></span>          | <span data-ttu-id="c33aa-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33aa-133">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c33aa-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="c33aa-134">Authorization</span></span> | <span data-ttu-id="c33aa-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c33aa-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c33aa-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c33aa-137">Request body</span></span>

<span data-ttu-id="c33aa-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c33aa-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c33aa-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c33aa-139">Response</span></span>

<span data-ttu-id="c33aa-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de [colocar](../resources/place.md) objetos no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c33aa-140">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c33aa-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c33aa-141">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="c33aa-142">Exemplo 1: listar todas as salas definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="c33aa-142">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="c33aa-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c33aa-143">Request</span></span>

<span data-ttu-id="c33aa-144">O exemplo a seguir mostra como obter todos os objetos de [sala](../resources/room.md) no locatário.</span><span class="sxs-lookup"><span data-stu-id="c33aa-144">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c33aa-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c33aa-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c33aa-146">C#</span><span class="sxs-lookup"><span data-stu-id="c33aa-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c33aa-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="c33aa-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c33aa-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c33aa-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c33aa-149">Java</span><span class="sxs-lookup"><span data-stu-id="c33aa-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c33aa-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="c33aa-150">Response</span></span>

<span data-ttu-id="c33aa-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c33aa-151">The following is an example of the response.</span></span>

><span data-ttu-id="c33aa-152">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c33aa-152">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c33aa-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c33aa-153">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="c33aa-154">Exemplo 2: listar todas as listas de salas definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="c33aa-154">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="c33aa-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c33aa-155">Request</span></span>

<span data-ttu-id="c33aa-156">O exemplo a seguir mostra como obter todos os [](../resources/roomlist.md) objetos RoomList no locatário.</span><span class="sxs-lookup"><span data-stu-id="c33aa-156">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c33aa-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c33aa-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c33aa-158">C#</span><span class="sxs-lookup"><span data-stu-id="c33aa-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c33aa-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="c33aa-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c33aa-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c33aa-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c33aa-161">Java</span><span class="sxs-lookup"><span data-stu-id="c33aa-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c33aa-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c33aa-162">Response</span></span>

<span data-ttu-id="c33aa-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c33aa-163">The following is an example of the response.</span></span>

><span data-ttu-id="c33aa-164">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c33aa-164">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c33aa-165">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c33aa-165">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="c33aa-166">Exemplo 3: listar salas contidas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="c33aa-166">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="c33aa-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c33aa-167">Request</span></span>

<span data-ttu-id="c33aa-168">O exemplo a seguir mostra como obter uma lista de objetos [Room](../resources/room.md) contidos em uma **salalist**.</span><span class="sxs-lookup"><span data-stu-id="c33aa-168">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="c33aa-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="c33aa-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c33aa-170">C#</span><span class="sxs-lookup"><span data-stu-id="c33aa-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c33aa-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="c33aa-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c33aa-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c33aa-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c33aa-173">Java</span><span class="sxs-lookup"><span data-stu-id="c33aa-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c33aa-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="c33aa-174">Response</span></span>

<span data-ttu-id="c33aa-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c33aa-175">The following is an example of the response.</span></span>

><span data-ttu-id="c33aa-176">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c33aa-176">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c33aa-177">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c33aa-177">All the properties will be returned from an actual call.</span></span>

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
