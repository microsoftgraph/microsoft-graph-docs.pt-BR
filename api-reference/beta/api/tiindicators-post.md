---
title: Criar indicador de inteligência de ameaças
description: Criar um novo tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: be0e89fd353cbe54a9f3d9d6dbb3108a1b4da8db
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981466"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="4d8ca-103">Criar indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="4d8ca-103">Create threat intelligence indicator</span></span>

<span data-ttu-id="4d8ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d8ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d8ca-105">Criar um novo objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="4d8ca-105">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d8ca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d8ca-106">Permissions</span></span>

<span data-ttu-id="4d8ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d8ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d8ca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d8ca-109">Permission type</span></span>                        | <span data-ttu-id="4d8ca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d8ca-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4d8ca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d8ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d8ca-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4d8ca-112">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="4d8ca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d8ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d8ca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d8ca-114">Not supported.</span></span> |
| <span data-ttu-id="4d8ca-115">Application</span><span class="sxs-lookup"><span data-stu-id="4d8ca-115">Application</span></span>                            | <span data-ttu-id="4d8ca-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4d8ca-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d8ca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d8ca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="4d8ca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d8ca-118">Request headers</span></span>

| <span data-ttu-id="4d8ca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4d8ca-119">Name</span></span>          | <span data-ttu-id="4d8ca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d8ca-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d8ca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d8ca-121">Authorization</span></span> | <span data-ttu-id="4d8ca-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4d8ca-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d8ca-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d8ca-123">Request body</span></span>

<span data-ttu-id="4d8ca-124">No corpo da solicitação, forneça uma representação JSON de um objeto [tiIndicator](../resources/tiindicator.md) que contém pelo menos um [email](../resources/tiindicator.md#indicator-observables---email), [arquivo](../resources/tiindicator.md#indicator-observables---file)ou [rede](../resources/tiindicator.md#indicator-observables---network) observou, e os seguintes campos obrigatórios:,,,, `action` `description` `expirationDateTime` `targetProduct` `threatType` , `tlpLevel` .</span><span class="sxs-lookup"><span data-stu-id="4d8ca-124">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span> 

## <a name="response"></a><span data-ttu-id="4d8ca-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d8ca-125">Response</span></span>

<span data-ttu-id="4d8ca-126">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d8ca-126">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d8ca-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4d8ca-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d8ca-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d8ca-128">Request</span></span>

<span data-ttu-id="4d8ca-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d8ca-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d8ca-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d8ca-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators
Content-type: application/json

{
  "action": "alert",
  "activityGroupNames": [],
  "confidence": 0,
  "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
  "expirationDateTime": "2019-03-01T21:43:37.5031462+00:00",
  "externalId": "Test--8586509942679764298MS501",
  "fileHashType": "sha256",
  "fileHashValue": "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
  "killChain": [],
  "malwareFamilyNames": [],
  "severity": 0,
  "tags": [],
  "targetProduct": "Azure Sentinel",
  "threatType": "WatchList",
  "tlpLevel": "green"
}
```
# <a name="c"></a>[<span data-ttu-id="4d8ca-131">C#</span><span class="sxs-lookup"><span data-stu-id="4d8ca-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d8ca-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d8ca-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d8ca-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d8ca-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d8ca-134">Java</span><span class="sxs-lookup"><span data-stu-id="4d8ca-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tiindicator-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d8ca-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d8ca-135">Response</span></span>

<span data-ttu-id="4d8ca-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d8ca-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4d8ca-137">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4d8ca-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4d8ca-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d8ca-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXX",
    "action": "alert",
    "additionalInformation": null,
    "activityGroupNames": [],
    "confidence": 0,
    "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


