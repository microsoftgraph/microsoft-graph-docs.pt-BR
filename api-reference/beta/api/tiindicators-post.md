---
title: Criar indicador de inteligência de ameaças
description: Criar um novo tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: af765b0cc90418e4c1115c7dde4438ed27a433d2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270599"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="91082-103">Criar indicador de inteligência de ameaças</span><span class="sxs-lookup"><span data-stu-id="91082-103">Create threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91082-104">Criar um novo objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="91082-104">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91082-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="91082-105">Permissions</span></span>

<span data-ttu-id="91082-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91082-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91082-108">Permission type</span></span>                        | <span data-ttu-id="91082-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91082-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="91082-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91082-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="91082-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="91082-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="91082-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91082-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91082-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91082-113">Not supported.</span></span> |
| <span data-ttu-id="91082-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91082-114">Application</span></span>                            | <span data-ttu-id="91082-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="91082-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="91082-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91082-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="91082-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91082-117">Request headers</span></span>

| <span data-ttu-id="91082-118">Nome</span><span class="sxs-lookup"><span data-stu-id="91082-118">Name</span></span>          | <span data-ttu-id="91082-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="91082-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="91082-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="91082-120">Authorization</span></span> | <span data-ttu-id="91082-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="91082-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="91082-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91082-122">Request body</span></span>

<span data-ttu-id="91082-123">No corpo da solicitação, forneça uma representação JSON de um objeto [tiIndicator](../resources/tiindicator.md) que contém pelo menos um [email](../resources/tiindicator.md#indicator-observables---email), [arquivo](../resources/tiindicator.md#indicator-observables---file)ou [rede](../resources/tiindicator.md#indicator-observables---network) observável.</span><span class="sxs-lookup"><span data-stu-id="91082-123">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable.</span></span>

## <a name="response"></a><span data-ttu-id="91082-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="91082-124">Response</span></span>

<span data-ttu-id="91082-125">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91082-125">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91082-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="91082-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91082-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91082-127">Request</span></span>

<span data-ttu-id="91082-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91082-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91082-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="91082-129">Response</span></span>

<span data-ttu-id="91082-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91082-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="91082-131">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="91082-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="91082-132">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91082-132">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="91082-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="91082-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="91082-134">C#</span><span class="sxs-lookup"><span data-stu-id="91082-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_tiindicator_from_security-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91082-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="91082-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_tiindicator_from_security-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="91082-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="91082-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_tiindicator_from_security-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicators-post.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicators-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicators-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
