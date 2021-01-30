---
title: Listar locais
description: Recupere uma lista de objetos de local.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6232c19bb3f9e1c8f24908b017625ec6cc00985b
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059732"
---
# <a name="list-places"></a><span data-ttu-id="21c83-103">Listar locais</span><span class="sxs-lookup"><span data-stu-id="21c83-103">List places</span></span>

<span data-ttu-id="21c83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21c83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21c83-105">Obter uma coleção do tipo especificado de objetos [de local](../resources/place.md) definidos no locatário.</span><span class="sxs-lookup"><span data-stu-id="21c83-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="21c83-106">Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.</span><span class="sxs-lookup"><span data-stu-id="21c83-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="21c83-107">Um **objeto** place pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="21c83-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="21c83-108">Uma [sala](../resources/room.md) que inclui propriedades rica, como um endereço de email para a sala e acessibilidade, capacidade e suporte ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21c83-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="21c83-109">Uma [lista de](../resources/roomlist.md) sala que inclui um endereço de email para a lista de sala e uma propriedade de navegação para obter a coleção de instâncias de sala na lista de sala.</span><span class="sxs-lookup"><span data-stu-id="21c83-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="21c83-110">Room **e** **roomList** são derivados do **objeto place.**</span><span class="sxs-lookup"><span data-stu-id="21c83-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="21c83-111">Por padrão, essa operação retorna 100 lugares por página.</span><span class="sxs-lookup"><span data-stu-id="21c83-111">By default, this operation returns 100 places per page.</span></span> 

<span data-ttu-id="21c83-112">Em comparação com [as funções findRooms](../api/user-findrooms.md) e [findRoomLists,](../api/user-findroomlists.md) essa operação retorna uma carga mais avançada para salas e listas de salas.</span><span class="sxs-lookup"><span data-stu-id="21c83-112">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="21c83-113">Veja [os detalhes](../resources/place.md#using-the-places-api) de como eles se comparam.</span><span class="sxs-lookup"><span data-stu-id="21c83-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="21c83-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="21c83-114">Permissions</span></span>

<span data-ttu-id="21c83-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21c83-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21c83-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21c83-117">Permission type</span></span>                        | <span data-ttu-id="21c83-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21c83-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="21c83-119">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21c83-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="21c83-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="21c83-120">Place.Read.All</span></span> |
| <span data-ttu-id="21c83-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21c83-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21c83-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="21c83-122">Not supported</span></span> |
| <span data-ttu-id="21c83-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21c83-123">Application</span></span>                            | <span data-ttu-id="21c83-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="21c83-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21c83-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21c83-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="21c83-126">Para obter todas as salas em um locatário:</span><span class="sxs-lookup"><span data-stu-id="21c83-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="21c83-127">Para obter todas as listas de sala em um locatário:</span><span class="sxs-lookup"><span data-stu-id="21c83-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="21c83-128">Para obter todas as salas na lista de salas especificada:</span><span class="sxs-lookup"><span data-stu-id="21c83-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="21c83-129">**Observação:** para obter salas em uma lista de salas, você deve especificar a lista de salas por sua **propriedade emailAddress,** não por **sua id**.</span><span class="sxs-lookup"><span data-stu-id="21c83-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="21c83-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21c83-130">Optional query parameters</span></span>
<span data-ttu-id="21c83-131">Esse método dá suporte aos seguintes parâmetros de consulta para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="21c83-131">This method supports the following query parameters to help customize the response:</span></span>
- <span data-ttu-id="21c83-132">$filter</span><span class="sxs-lookup"><span data-stu-id="21c83-132">$filter</span></span>
- <span data-ttu-id="21c83-133">$select</span><span class="sxs-lookup"><span data-stu-id="21c83-133">$select</span></span>
- <span data-ttu-id="21c83-134">$top</span><span class="sxs-lookup"><span data-stu-id="21c83-134">$top</span></span>
- <span data-ttu-id="21c83-135">$skip</span><span class="sxs-lookup"><span data-stu-id="21c83-135">$skip</span></span>
- <span data-ttu-id="21c83-136">$count=true</span><span class="sxs-lookup"><span data-stu-id="21c83-136">$count=true</span></span>

<span data-ttu-id="21c83-137">Use $top para personalizar o tamanho da página.</span><span class="sxs-lookup"><span data-stu-id="21c83-137">Use $top to customize the page size.</span></span> <span data-ttu-id="21c83-138">O tamanho de página padrão é 100.</span><span class="sxs-lookup"><span data-stu-id="21c83-138">The default page size is 100.</span></span>

<span data-ttu-id="21c83-139">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="21c83-139">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="21c83-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21c83-140">Request headers</span></span>

| <span data-ttu-id="21c83-141">Nome</span><span class="sxs-lookup"><span data-stu-id="21c83-141">Name</span></span>          | <span data-ttu-id="21c83-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="21c83-142">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="21c83-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="21c83-143">Authorization</span></span> | <span data-ttu-id="21c83-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21c83-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21c83-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21c83-146">Request body</span></span>

<span data-ttu-id="21c83-147">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21c83-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21c83-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="21c83-148">Response</span></span>

<span data-ttu-id="21c83-149">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de objetos [place](../resources/place.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21c83-149">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21c83-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="21c83-150">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="21c83-151">Exemplo 1: Listar todas as salas definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="21c83-151">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="21c83-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21c83-152">Request</span></span>

<span data-ttu-id="21c83-153">O exemplo a seguir mostra como obter todos os [objetos de](../resources/room.md) sala no locatário.</span><span class="sxs-lookup"><span data-stu-id="21c83-153">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="21c83-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="21c83-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```
# <a name="c"></a>[<span data-ttu-id="21c83-155">C#</span><span class="sxs-lookup"><span data-stu-id="21c83-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21c83-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21c83-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21c83-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21c83-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21c83-158">Java</span><span class="sxs-lookup"><span data-stu-id="21c83-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21c83-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="21c83-159">Response</span></span>

<span data-ttu-id="21c83-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21c83-160">The following is an example of the response.</span></span>

><span data-ttu-id="21c83-161">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21c83-161">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="21c83-162">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21c83-162">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="21c83-163">Exemplo 2: Listar todas as listas de sala definidas no locatário</span><span class="sxs-lookup"><span data-stu-id="21c83-163">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="21c83-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21c83-164">Request</span></span>

<span data-ttu-id="21c83-165">O exemplo a seguir mostra como obter todos os [objetos roomList](../resources/roomlist.md) no locatário.</span><span class="sxs-lookup"><span data-stu-id="21c83-165">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="21c83-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="21c83-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```
# <a name="c"></a>[<span data-ttu-id="21c83-167">C#</span><span class="sxs-lookup"><span data-stu-id="21c83-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21c83-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21c83-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21c83-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21c83-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21c83-170">Java</span><span class="sxs-lookup"><span data-stu-id="21c83-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21c83-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="21c83-171">Response</span></span>

<span data-ttu-id="21c83-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21c83-172">The following is an example of the response.</span></span>

><span data-ttu-id="21c83-173">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21c83-173">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="21c83-174">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21c83-174">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="21c83-175">Exemplo 3: Listar salas contidas em uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="21c83-175">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="21c83-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21c83-176">Request</span></span>

<span data-ttu-id="21c83-177">O exemplo a seguir mostra como obter uma lista de objetos [de sala](../resources/room.md) contidos em uma **roomList**.</span><span class="sxs-lookup"><span data-stu-id="21c83-177">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="21c83-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="21c83-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="c"></a>[<span data-ttu-id="21c83-179">C#</span><span class="sxs-lookup"><span data-stu-id="21c83-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21c83-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21c83-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21c83-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21c83-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21c83-182">Java</span><span class="sxs-lookup"><span data-stu-id="21c83-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21c83-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="21c83-183">Response</span></span>

<span data-ttu-id="21c83-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21c83-184">The following is an example of the response.</span></span>

><span data-ttu-id="21c83-185">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21c83-185">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="21c83-186">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21c83-186">All the properties will be returned from an actual call.</span></span>

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
    "Error: Malformed function params 'id-of-roomlist'"
  ]
}-->


