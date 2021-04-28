---
title: Listar locais
description: Recupere uma lista de objetos de local.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c6c128b9aca8f8ef455a70f92f43b27c8d325525
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053976"
---
# <a name="list-places"></a><span data-ttu-id="d15ad-103">Listar locais</span><span class="sxs-lookup"><span data-stu-id="d15ad-103">List places</span></span>

<span data-ttu-id="d15ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d15ad-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d15ad-105">Obter uma coleção do tipo especificado de [objetos de local](../resources/place.md) definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="d15ad-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="d15ad-106">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="d15ad-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="d15ad-107">Um **objeto place** pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="d15ad-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="d15ad-108">Uma [sala](../resources/room.md) que inclui propriedades ricas, como um endereço de email para a sala e acessibilidade, capacidade e suporte a dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d15ad-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="d15ad-109">Uma [lista de](../resources/roomlist.md) sala que inclui um endereço de email para a lista de sala e uma propriedade de navegação para obter a coleção de instâncias de sala na lista de sala.</span><span class="sxs-lookup"><span data-stu-id="d15ad-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span>

<span data-ttu-id="d15ad-110">Sala **e** **roomList** são derivados do **objeto place.**</span><span class="sxs-lookup"><span data-stu-id="d15ad-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="d15ad-111">Por padrão, essa operação retorna 100 locais por página.</span><span class="sxs-lookup"><span data-stu-id="d15ad-111">By default, this operation returns 100 places per page.</span></span>

<span data-ttu-id="d15ad-112">Em comparação com [as funções findRooms](/graph/api/user-findrooms?view=graph-rest-beta) e [findRoomLists,](/graph/api/user-findroomlists?view=graph-rest-beta) essa operação retorna uma carga mais rica para salas e listas de salas.</span><span class="sxs-lookup"><span data-stu-id="d15ad-112">Compared with the [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) and [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="d15ad-113">Confira [detalhes](../resources/place.md#using-the-places-api) sobre como eles se comparam.</span><span class="sxs-lookup"><span data-stu-id="d15ad-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="d15ad-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="d15ad-114">Permissions</span></span>

<span data-ttu-id="d15ad-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d15ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d15ad-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d15ad-117">Permission type</span></span>                        | <span data-ttu-id="d15ad-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d15ad-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d15ad-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d15ad-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="d15ad-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="d15ad-120">Place.Read.All</span></span> |
| <span data-ttu-id="d15ad-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d15ad-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d15ad-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d15ad-122">Not supported</span></span> |
| <span data-ttu-id="d15ad-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d15ad-123">Application</span></span>                            | <span data-ttu-id="d15ad-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="d15ad-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d15ad-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d15ad-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d15ad-126">Para obter todas as salas em um locatário:</span><span class="sxs-lookup"><span data-stu-id="d15ad-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="d15ad-127">Para obter todas as listas de sala em um locatário:</span><span class="sxs-lookup"><span data-stu-id="d15ad-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="d15ad-128">Para obter todas as salas na lista de salas especificada:</span><span class="sxs-lookup"><span data-stu-id="d15ad-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="d15ad-129">**Observação**: para obter salas em uma lista de salas, você deve especificar a lista de salas por sua **propriedade emailAddress,** não por **sua id**.</span><span class="sxs-lookup"><span data-stu-id="d15ad-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d15ad-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d15ad-130">Optional query parameters</span></span>
<span data-ttu-id="d15ad-131">Este método dá suporte aos seguintes parâmetros de consulta para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="d15ad-131">This method supports the following query parameters to help customize the response:</span></span>
- `$filter`
- `$select`
- `$top`
- `$skip`
- `$count=true`

<span data-ttu-id="d15ad-132">Use `$top` para personalizar o tamanho da página.</span><span class="sxs-lookup"><span data-stu-id="d15ad-132">Use `$top` to customize the page size.</span></span> <span data-ttu-id="d15ad-133">O tamanho de página padrão é 100.</span><span class="sxs-lookup"><span data-stu-id="d15ad-133">The default page size is 100.</span></span>

<span data-ttu-id="d15ad-134">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d15ad-134">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d15ad-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d15ad-135">Request headers</span></span>

| <span data-ttu-id="d15ad-136">Nome</span><span class="sxs-lookup"><span data-stu-id="d15ad-136">Name</span></span>          | <span data-ttu-id="d15ad-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d15ad-137">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d15ad-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="d15ad-138">Authorization</span></span> | <span data-ttu-id="d15ad-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d15ad-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d15ad-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d15ad-141">Request body</span></span>

<span data-ttu-id="d15ad-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d15ad-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d15ad-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d15ad-143">Response</span></span>

<span data-ttu-id="d15ad-144">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [place](../resources/place.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d15ad-144">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d15ad-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d15ad-145">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="d15ad-146">Exemplo 1: Listar todas as salas definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="d15ad-146">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="d15ad-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d15ad-147">Request</span></span>

<span data-ttu-id="d15ad-148">O exemplo a seguir mostra como obter todos os objetos [de](../resources/room.md) sala no locatário.</span><span class="sxs-lookup"><span data-stu-id="d15ad-148">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>



# <a name="http"></a>[<span data-ttu-id="d15ad-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d15ad-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.room
```
# <a name="c"></a>[<span data-ttu-id="d15ad-150">C#</span><span class="sxs-lookup"><span data-stu-id="d15ad-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d15ad-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d15ad-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d15ad-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d15ad-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d15ad-153">Java</span><span class="sxs-lookup"><span data-stu-id="d15ad-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d15ad-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d15ad-154">Response</span></span>

<span data-ttu-id="d15ad-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d15ad-155">The following is an example of the response.</span></span>

><span data-ttu-id="d15ad-156">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d15ad-156">**Note**: The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/microsoft.graph.room",
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
      "capacity": 50,
      "building": "1",
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
      "capacity": 40,
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelChairAccessible": false,
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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="d15ad-157">Exemplo 2: Listar todas as listas de sala definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="d15ad-157">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="d15ad-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d15ad-158">Request</span></span>

<span data-ttu-id="d15ad-159">O exemplo a seguir mostra como obter todos os [objetos roomList](../resources/roomlist.md) no locatário.</span><span class="sxs-lookup"><span data-stu-id="d15ad-159">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="d15ad-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d15ad-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.roomlist
```
# <a name="c"></a>[<span data-ttu-id="d15ad-161">C#</span><span class="sxs-lookup"><span data-stu-id="d15ad-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d15ad-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d15ad-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d15ad-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d15ad-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d15ad-164">Java</span><span class="sxs-lookup"><span data-stu-id="d15ad-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d15ad-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d15ad-165">Response</span></span>

<span data-ttu-id="d15ad-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d15ad-166">The following is an example of the response.</span></span>

><span data-ttu-id="d15ad-167">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d15ad-167">**Note**: The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/microsoft.graph.roomList",
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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="d15ad-168">Exemplo 3: Listar salas contidas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="d15ad-168">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="d15ad-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d15ad-169">Request</span></span>

<span data-ttu-id="d15ad-170">O exemplo a seguir mostra como obter uma lista de objetos [de](../resources/room.md) sala contidos em uma **roomList**.</span><span class="sxs-lookup"><span data-stu-id="d15ad-170">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span>


# <a name="http"></a>[<span data-ttu-id="d15ad-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="d15ad-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="c"></a>[<span data-ttu-id="d15ad-172">C#</span><span class="sxs-lookup"><span data-stu-id="d15ad-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d15ad-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d15ad-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d15ad-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d15ad-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d15ad-175">Java</span><span class="sxs-lookup"><span data-stu-id="d15ad-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d15ad-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="d15ad-176">Response</span></span>

<span data-ttu-id="d15ad-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d15ad-177">The following is an example of the response.</span></span>

><span data-ttu-id="d15ad-178">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d15ad-178">**Note**: The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places('bldg2%40contoso.com')/microsoft.graph.roomList/rooms",
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
      "capacity": 40,
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelChairAccessible": false,
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
  ]
}-->
