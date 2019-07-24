---
title: Obter local
description: Recupere as propriedades e os relacionamentos de um objeto local.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b53f6b1cb89bb4c5b3d02d5b32154877a5de706
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841063"
---
# <a name="get-place"></a><span data-ttu-id="db9e1-103">Obter local</span><span class="sxs-lookup"><span data-stu-id="db9e1-103">Get place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="db9e1-104">Obtenha as propriedades e os relacionamentos de um objeto [local](../resources/place.md) especificado por sua ID ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="db9e1-104">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="db9e1-105">O objeto **local** pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="db9e1-105">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="db9e1-106">Uma [sala](../resources/room.md) que inclui Propriedades sofisticadas, como um endereço de email para a sala, e suporte à acessibilidade, capacidade e dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db9e1-106">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="db9e1-107">Uma [lista de salas](../resources/roomlist.md) que inclui um endereço de email para a lista de salas e uma propriedade de navegação para obter a coleção de instâncias de **sala** na lista de salas.</span><span class="sxs-lookup"><span data-stu-id="db9e1-107">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="db9e1-108">A **sala** e \*\*\*\* a salalist são derivadas do objeto [local](../resources/place.md) .</span><span class="sxs-lookup"><span data-stu-id="db9e1-108">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="db9e1-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="db9e1-109">Permissions</span></span>

<span data-ttu-id="db9e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db9e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db9e1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db9e1-112">Permission type</span></span>                        | <span data-ttu-id="db9e1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db9e1-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db9e1-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db9e1-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="db9e1-115">Local. Read. All</span><span class="sxs-lookup"><span data-stu-id="db9e1-115">Place.Read.All</span></span> |
| <span data-ttu-id="db9e1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db9e1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db9e1-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db9e1-117">Not supported</span></span> |
| <span data-ttu-id="db9e1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db9e1-118">Application</span></span>                            | <span data-ttu-id="db9e1-119">Local. Read. All</span><span class="sxs-lookup"><span data-stu-id="db9e1-119">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db9e1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db9e1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db9e1-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="db9e1-121">Optional query parameters</span></span>

<span data-ttu-id="db9e1-122">Este método dá suporte aos seguintes parâmetros de consulta para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="db9e1-122">This method supports the following query parameters to help customize the response:</span></span>
* <span data-ttu-id="db9e1-123">$filter</span><span class="sxs-lookup"><span data-stu-id="db9e1-123">$filter</span></span>
* <span data-ttu-id="db9e1-124">$select</span><span class="sxs-lookup"><span data-stu-id="db9e1-124">$select</span></span>
* <span data-ttu-id="db9e1-125">$top</span><span class="sxs-lookup"><span data-stu-id="db9e1-125">$top</span></span>

<span data-ttu-id="db9e1-126">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="db9e1-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="db9e1-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db9e1-127">Request headers</span></span>

| <span data-ttu-id="db9e1-128">Nome</span><span class="sxs-lookup"><span data-stu-id="db9e1-128">Name</span></span>          | <span data-ttu-id="db9e1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="db9e1-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="db9e1-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="db9e1-130">Authorization</span></span> | <span data-ttu-id="db9e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db9e1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db9e1-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db9e1-133">Request body</span></span>

<span data-ttu-id="db9e1-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db9e1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db9e1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9e1-135">Response</span></span>

<span data-ttu-id="db9e1-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [local](../resources/place.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db9e1-136">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db9e1-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db9e1-137">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="db9e1-138">Exemplo 1: obter uma sala</span><span class="sxs-lookup"><span data-stu-id="db9e1-138">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="db9e1-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db9e1-139">Request</span></span>

<span data-ttu-id="db9e1-140">O exemplo a seguir especifica a **ID** de uma **sala** para obter suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="db9e1-140">The following example specifies the **id** of a **room** to get its properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```http
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```

#### <a name="response"></a><span data-ttu-id="db9e1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9e1-141">Response</span></span>

<span data-ttu-id="db9e1-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db9e1-142">The following is an example of the response.</span></span>

><span data-ttu-id="db9e1-143">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db9e1-143">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db9e1-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db9e1-144">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="db9e1-145">Exemplo 2: obter uma lista de salas</span><span class="sxs-lookup"><span data-stu-id="db9e1-145">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="db9e1-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db9e1-146">Request</span></span>

<span data-ttu-id="db9e1-147">O exemplo a seguir especifica o **EmailAddress** de uma **RoomList** para obter suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="db9e1-147">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```

#### <a name="response"></a><span data-ttu-id="db9e1-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9e1-148">Response</span></span>

<span data-ttu-id="db9e1-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db9e1-149">The following is an example of the response.</span></span>

><span data-ttu-id="db9e1-150">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db9e1-150">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db9e1-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db9e1-151">All the properties will be returned from an actual call.</span></span>

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
