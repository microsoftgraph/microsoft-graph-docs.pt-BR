---
title: Obter local
description: Recupere as propriedades e os relacionamentos de um objeto local.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3934a6cbb683e6bd6591e2dfcc33f8361bc4d0e5
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290480"
---
# <a name="get-place"></a><span data-ttu-id="f589b-103">Obter local</span><span class="sxs-lookup"><span data-stu-id="f589b-103">Get place</span></span>

<span data-ttu-id="f589b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f589b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f589b-105">Obtenha as propriedades e os relacionamentos de um objeto [local](../resources/place.md) especificado por sua ID ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="f589b-105">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="f589b-106">O objeto **local** pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="f589b-106">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="f589b-107">Uma [sala](../resources/room.md) que inclui Propriedades sofisticadas, como um endereço de email para a sala, e suporte à acessibilidade, capacidade e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f589b-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="f589b-108">Uma [lista de salas](../resources/roomlist.md) que inclui um endereço de email para a lista de salas e uma propriedade de navegação para obter a coleção de instâncias de **sala** na lista de salas.</span><span class="sxs-lookup"><span data-stu-id="f589b-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="f589b-109">A **sala** e a **salalist** são derivadas do objeto [local](../resources/place.md) .</span><span class="sxs-lookup"><span data-stu-id="f589b-109">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f589b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f589b-110">Permissions</span></span>

<span data-ttu-id="f589b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f589b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f589b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f589b-113">Permission type</span></span>                        | <span data-ttu-id="f589b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f589b-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f589b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f589b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="f589b-116">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="f589b-116">Place.Read.All</span></span> |
| <span data-ttu-id="f589b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f589b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f589b-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f589b-118">Not supported</span></span> |
| <span data-ttu-id="f589b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f589b-119">Application</span></span>                            | <span data-ttu-id="f589b-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="f589b-120">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f589b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f589b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f589b-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f589b-122">Optional query parameters</span></span>
<span data-ttu-id="f589b-123">Use `$select` para obter propriedades de **local** específico.</span><span class="sxs-lookup"><span data-stu-id="f589b-123">Use `$select` to get specific **place** properties.</span></span>

<span data-ttu-id="f589b-124">Para obter mais informações, consulte [OData Query Parameters](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f589b-124">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f589b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f589b-125">Request headers</span></span>

| <span data-ttu-id="f589b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="f589b-126">Name</span></span>          | <span data-ttu-id="f589b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f589b-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f589b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f589b-128">Authorization</span></span> | <span data-ttu-id="f589b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f589b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f589b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f589b-131">Request body</span></span>

<span data-ttu-id="f589b-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f589b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f589b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f589b-133">Response</span></span>

<span data-ttu-id="f589b-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [local](../resources/place.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f589b-134">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f589b-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f589b-135">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="f589b-136">Exemplo 1: obter uma sala</span><span class="sxs-lookup"><span data-stu-id="f589b-136">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="f589b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f589b-137">Request</span></span>

<span data-ttu-id="f589b-138">O exemplo a seguir especifica a **ID** de uma **sala** para obter suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f589b-138">The following example specifies the **id** of a **room** to get its properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```

#### <a name="response"></a><span data-ttu-id="f589b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f589b-139">Response</span></span>

<span data-ttu-id="f589b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f589b-140">The following is an example of the response.</span></span>

><span data-ttu-id="f589b-141">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f589b-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f589b-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f589b-142">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="f589b-143">Exemplo 2: obter uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="f589b-143">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="f589b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f589b-144">Request</span></span>

<span data-ttu-id="f589b-145">O exemplo a seguir especifica o **EmailAddress** de uma **RoomList** para obter suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f589b-145">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg1@contoso.com
```


#### <a name="response"></a><span data-ttu-id="f589b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f589b-146">Response</span></span>

<span data-ttu-id="f589b-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f589b-147">The following is an example of the response.</span></span>

><span data-ttu-id="f589b-148">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f589b-148">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f589b-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f589b-149">All the properties will be returned from an actual call.</span></span>

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
