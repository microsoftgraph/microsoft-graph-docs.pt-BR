---
title: Criar namedLocation
description: Criar um novo namedLocation.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 99b81875c2d7df1f2b8f5fabd164c626f7af6a26
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384442"
---
# <a name="create-namedlocation"></a><span data-ttu-id="f54c5-103">Criar namedLocation</span><span class="sxs-lookup"><span data-stu-id="f54c5-103">Create namedLocation</span></span>

<span data-ttu-id="f54c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f54c5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f54c5-105">Criar um novo objeto [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="f54c5-105">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f54c5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f54c5-106">Permissions</span></span>

<span data-ttu-id="f54c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f54c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f54c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f54c5-109">Permission type</span></span>                        | <span data-ttu-id="f54c5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f54c5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f54c5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f54c5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f54c5-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="f54c5-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="f54c5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f54c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f54c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f54c5-114">Not supported.</span></span> |
| <span data-ttu-id="f54c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f54c5-115">Application</span></span>                            | <span data-ttu-id="f54c5-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="f54c5-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="f54c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f54c5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="f54c5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f54c5-118">Request headers</span></span>

| <span data-ttu-id="f54c5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f54c5-119">Name</span></span>          | <span data-ttu-id="f54c5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f54c5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f54c5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f54c5-121">Authorization</span></span> | <span data-ttu-id="f54c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f54c5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f54c5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f54c5-124">Content-Type</span></span>  | <span data-ttu-id="f54c5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f54c5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f54c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f54c5-127">Request body</span></span>

<span data-ttu-id="f54c5-128">No corpo da solicitação, forneça uma representação JSON de um objeto [ipNamedLocation](../resources/ipnamedlocation.md) ou [countryNamedLocation](../resources/countrynamedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="f54c5-128">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f54c5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f54c5-129">Response</span></span>

<span data-ttu-id="f54c5-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [IpNamedLocation](../resources/ipnamedlocation.md) ou [countryNamedLocation](../resources/countrynamedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f54c5-130">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f54c5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f54c5-131">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="f54c5-132">Exemplo 1: criar um ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="f54c5-132">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="f54c5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f54c5-133">Request</span></span>

<span data-ttu-id="f54c5-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f54c5-134">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="f54c5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f54c5-135">Response</span></span>

<span data-ttu-id="f54c5-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f54c5-136">The following is an example of the response.</span></span>

> <span data-ttu-id="f54c5-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f54c5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="f54c5-139">Exemplo 2: criar um countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="f54c5-139">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="f54c5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f54c5-140">Request</span></span>

<span data-ttu-id="f54c5-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f54c5-141">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="f54c5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f54c5-142">Response</span></span>

<span data-ttu-id="f54c5-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f54c5-143">The following is an example of the response.</span></span>

> <span data-ttu-id="f54c5-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f54c5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
