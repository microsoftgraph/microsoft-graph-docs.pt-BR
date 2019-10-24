---
title: Criar namedLocation
description: Criar um novo namedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5d6962a9cae9eb3a49177ecaa4d17a0c4181881
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653724"
---
# <a name="create-namedlocation"></a><span data-ttu-id="83eaf-103">Criar namedLocation</span><span class="sxs-lookup"><span data-stu-id="83eaf-103">Create namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83eaf-104">Criar um novo objeto [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="83eaf-104">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="83eaf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="83eaf-105">Permissions</span></span>

<span data-ttu-id="83eaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83eaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83eaf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83eaf-108">Permission type</span></span>                        | <span data-ttu-id="83eaf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83eaf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83eaf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83eaf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="83eaf-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="83eaf-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="83eaf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83eaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83eaf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83eaf-113">Not supported.</span></span> |
| <span data-ttu-id="83eaf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83eaf-114">Application</span></span>                            | <span data-ttu-id="83eaf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83eaf-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="83eaf-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="83eaf-116">This API requires multiple permissions.</span></span> <span data-ttu-id="83eaf-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="83eaf-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="83eaf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83eaf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="83eaf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83eaf-119">Request headers</span></span>

| <span data-ttu-id="83eaf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="83eaf-120">Name</span></span>          | <span data-ttu-id="83eaf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="83eaf-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="83eaf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="83eaf-122">Authorization</span></span> | <span data-ttu-id="83eaf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83eaf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83eaf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83eaf-125">Content-Type</span></span>  | <span data-ttu-id="83eaf-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83eaf-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83eaf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83eaf-128">Request body</span></span>

<span data-ttu-id="83eaf-129">No corpo da solicitação, forneça uma representação JSON de um objeto [ipNamedLocation](../resources/ipnamedlocation.md) ou [countryNamedLocation](../resources/countrynamedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="83eaf-129">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="83eaf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="83eaf-130">Response</span></span>

<span data-ttu-id="83eaf-131">Se tiver êxito, este método retornará `201 Created`um código de resposta e um novo objeto [ipNamedLocation](../resources/ipnamedlocation.md) ou [countryNamedLocation](../resources/countrynamedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83eaf-131">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83eaf-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="83eaf-132">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="83eaf-133">Exemplo 1: criar um ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="83eaf-133">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="83eaf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83eaf-134">Request</span></span>

<span data-ttu-id="83eaf-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83eaf-135">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="83eaf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="83eaf-136">Response</span></span>

<span data-ttu-id="83eaf-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83eaf-137">The following is an example of the response.</span></span>

> <span data-ttu-id="83eaf-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83eaf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="83eaf-140">Exemplo 2: criar um countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="83eaf-140">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="83eaf-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83eaf-141">Request</span></span>

<span data-ttu-id="83eaf-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83eaf-142">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="83eaf-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="83eaf-143">Response</span></span>

<span data-ttu-id="83eaf-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83eaf-144">The following is an example of the response.</span></span>

> <span data-ttu-id="83eaf-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83eaf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
