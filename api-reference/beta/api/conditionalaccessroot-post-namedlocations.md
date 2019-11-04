---
title: Criar namedLocation
description: Criar um novo namedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a588dc58df43e818ab4b1c2c239cb81b3ec8b4e1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936628"
---
# <a name="create-namedlocation"></a><span data-ttu-id="f5f2f-103">Criar namedLocation</span><span class="sxs-lookup"><span data-stu-id="f5f2f-103">Create namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5f2f-104">Criar um novo objeto [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="f5f2f-104">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5f2f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5f2f-105">Permissions</span></span>

<span data-ttu-id="f5f2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5f2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5f2f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5f2f-108">Permission type</span></span>                        | <span data-ttu-id="f5f2f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5f2f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f5f2f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5f2f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5f2f-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f5f2f-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f5f2f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5f2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5f2f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-113">Not supported.</span></span> |
| <span data-ttu-id="f5f2f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5f2f-114">Application</span></span>                            | <span data-ttu-id="f5f2f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="f5f2f-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-116">This API requires multiple permissions.</span></span> <span data-ttu-id="f5f2f-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="f5f2f-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="f5f2f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f2f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="f5f2f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f2f-119">Request headers</span></span>

| <span data-ttu-id="f5f2f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f5f2f-120">Name</span></span>          | <span data-ttu-id="f5f2f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5f2f-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f5f2f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5f2f-122">Authorization</span></span> | <span data-ttu-id="f5f2f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5f2f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5f2f-125">Content-Type</span></span>  | <span data-ttu-id="f5f2f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5f2f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f2f-128">Request body</span></span>

<span data-ttu-id="f5f2f-129">No corpo da solicitação, forneça uma representação JSON de um objeto [ipNamedLocation](../resources/ipnamedlocation.md) ou [countryNamedLocation](../resources/countrynamedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="f5f2f-129">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f5f2f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f2f-130">Response</span></span>

<span data-ttu-id="f5f2f-131">Se tiver êxito, este método retornará `201 Created`um código de resposta e um novo objeto [ipNamedLocation](../resources/ipnamedlocation.md) ou [countryNamedLocation](../resources/countrynamedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-131">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5f2f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5f2f-132">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="f5f2f-133">Exemplo 1: criar um ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="f5f2f-133">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="f5f2f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f2f-134">Request</span></span>

<span data-ttu-id="f5f2f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f5f2f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f2f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/namedLocations
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5f2f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5f2f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-namedlocation-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f5f2f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5f2f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-namedlocation-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f5f2f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f2f-139">Response</span></span>

<span data-ttu-id="f5f2f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-140">The following is an example of the response.</span></span>

> <span data-ttu-id="f5f2f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
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
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="f5f2f-143">Exemplo 2: criar um countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="f5f2f-143">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="f5f2f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f2f-144">Request</span></span>

<span data-ttu-id="f5f2f-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/namedLocations
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

#### <a name="response"></a><span data-ttu-id="f5f2f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f2f-146">Response</span></span>

<span data-ttu-id="f5f2f-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-147">The following is an example of the response.</span></span>

> <span data-ttu-id="f5f2f-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f2f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
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
