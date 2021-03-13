---
title: Criar namedLocation
description: Crie um novo namedLocation.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bd716709ddd12a44814b24f58c9adb53701737d9
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761693"
---
# <a name="create-namedlocation"></a><span data-ttu-id="e69ed-103">Criar namedLocation</span><span class="sxs-lookup"><span data-stu-id="e69ed-103">Create namedLocation</span></span>

<span data-ttu-id="e69ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e69ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e69ed-105">Crie um novo [objeto namedLocation.](../resources/namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="e69ed-105">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e69ed-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e69ed-106">Permissions</span></span>

<span data-ttu-id="e69ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e69ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e69ed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e69ed-109">Permission type</span></span>                        | <span data-ttu-id="e69ed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e69ed-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e69ed-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e69ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e69ed-112">Policy.Read.All e Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="e69ed-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="e69ed-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e69ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e69ed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e69ed-114">Not supported.</span></span> |
| <span data-ttu-id="e69ed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e69ed-115">Application</span></span>                            | <span data-ttu-id="e69ed-116">Policy.Read.All e Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="e69ed-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="e69ed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e69ed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="e69ed-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e69ed-118">Request headers</span></span>

| <span data-ttu-id="e69ed-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e69ed-119">Name</span></span>          | <span data-ttu-id="e69ed-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e69ed-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e69ed-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e69ed-121">Authorization</span></span> | <span data-ttu-id="e69ed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e69ed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e69ed-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e69ed-124">Content-Type</span></span>  | <span data-ttu-id="e69ed-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e69ed-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e69ed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e69ed-127">Request body</span></span>

<span data-ttu-id="e69ed-128">No corpo da solicitação, fornece uma representação JSON de [um objeto ipNamedLocation](../resources/ipnamedlocation.md) [ou countryNamedLocation.](../resources/countrynamedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="e69ed-128">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e69ed-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69ed-129">Response</span></span>

<span data-ttu-id="e69ed-130">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto ipNamedLocation](../resources/ipnamedlocation.md) ou [countryNamedLocation](../resources/countrynamedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e69ed-130">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e69ed-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e69ed-131">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="e69ed-132">Exemplo 1: Criar um ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69ed-132">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="e69ed-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e69ed-133">Request</span></span>

<span data-ttu-id="e69ed-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e69ed-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e69ed-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e69ed-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "displayName": "Untrusted IP named location",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="e69ed-136">C#</span><span class="sxs-lookup"><span data-stu-id="e69ed-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-namedlocation-from-conditionalaccessroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e69ed-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e69ed-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-namedlocation-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e69ed-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e69ed-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-namedlocation-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e69ed-139">Java</span><span class="sxs-lookup"><span data-stu-id="e69ed-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-namedlocation-from-conditionalaccessroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e69ed-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69ed-140">Response</span></span>

<span data-ttu-id="e69ed-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e69ed-141">The following is an example of the response.</span></span>

> <span data-ttu-id="e69ed-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e69ed-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "id": "0854951d-5fc0-4eb1-b392-9b2c9d7949c2",
    "displayName": "Untrusted IP named location",
    "modifiedDateTime": "2019-09-04T01:11:34.9387578Z",
    "createdDateTime": "2019-09-04T01:11:34.9387578Z",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="e69ed-144">Exemplo 2: Criar um countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69ed-144">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="e69ed-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e69ed-145">Request</span></span>

<span data-ttu-id="e69ed-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e69ed-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Named location with unknown countries and regions",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```

#### <a name="response"></a><span data-ttu-id="e69ed-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e69ed-147">Response</span></span>

<span data-ttu-id="e69ed-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e69ed-148">The following is an example of the response.</span></span>

> <span data-ttu-id="e69ed-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e69ed-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "id": "1c4427fd-0885-4a3d-8b23-09a899ffa959",
    "displayName": "Named location with unknown countries and regions",
    "modifiedDateTime": "2019-09-04T01:08:02.5249255Z",
    "createdDateTime": "2019-09-04T01:08:02.5249255Z",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

