---
title: Criar indicador de inteligência de ameaças
description: Criar um novo tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 1400d880885c0f2c929d7ef7e448cfcf15789f8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990684"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="0f232-103">Criar indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="0f232-103">Create threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f232-104">Criar um novo objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="0f232-104">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f232-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f232-105">Permissions</span></span>

<span data-ttu-id="0f232-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f232-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f232-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f232-108">Permission type</span></span>                        | <span data-ttu-id="0f232-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f232-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f232-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f232-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f232-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0f232-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="0f232-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f232-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f232-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f232-113">Not supported.</span></span> |
| <span data-ttu-id="0f232-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f232-114">Application</span></span>                            | <span data-ttu-id="0f232-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0f232-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f232-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f232-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="0f232-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f232-117">Request headers</span></span>

| <span data-ttu-id="0f232-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0f232-118">Name</span></span>          | <span data-ttu-id="0f232-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f232-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0f232-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f232-120">Authorization</span></span> | <span data-ttu-id="0f232-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0f232-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f232-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f232-122">Request body</span></span>

<span data-ttu-id="0f232-123">No corpo da solicitação, forneça uma representação JSON de um objeto [tiIndicator](../resources/tiindicator.md) que contém pelo menos um [email](../resources/tiindicator.md#indicator-observables---email), [arquivo](../resources/tiindicator.md#indicator-observables---file)ou [rede](../resources/tiindicator.md#indicator-observables---network) observável.</span><span class="sxs-lookup"><span data-stu-id="0f232-123">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable.</span></span>

## <a name="response"></a><span data-ttu-id="0f232-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f232-124">Response</span></span>

<span data-ttu-id="0f232-125">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f232-125">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f232-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0f232-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f232-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f232-127">Request</span></span>

<span data-ttu-id="0f232-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f232-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0f232-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f232-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f232-130">C#</span><span class="sxs-lookup"><span data-stu-id="0f232-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f232-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="0f232-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f232-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f232-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0f232-133">Java</span><span class="sxs-lookup"><span data-stu-id="0f232-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tiindicator-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f232-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f232-134">Response</span></span>

<span data-ttu-id="0f232-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f232-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="0f232-136">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0f232-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0f232-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f232-137">All the properties will be returned from an actual call.</span></span>

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
