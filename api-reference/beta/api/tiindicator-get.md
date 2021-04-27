---
title: Obter indicador de inteligência de ameaça
description: Recupere as propriedades e as relações de um objeto tiindicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 7ae7d1dc59493454a3fef55948bb712a3aa1c772
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036398"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="143d0-103">Obter indicador de inteligência de ameaça</span><span class="sxs-lookup"><span data-stu-id="143d0-103">Get threat intelligence indicator</span></span>

<span data-ttu-id="143d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="143d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="143d0-105">Recupere as propriedades e as relações de um [objeto tiIndicator.](../resources/tiindicator.md)</span><span class="sxs-lookup"><span data-stu-id="143d0-105">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="143d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="143d0-106">Permissions</span></span>

<span data-ttu-id="143d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="143d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="143d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="143d0-109">Permission type</span></span>                        | <span data-ttu-id="143d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="143d0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="143d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="143d0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="143d0-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="143d0-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="143d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="143d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="143d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="143d0-114">Not supported.</span></span> |
| <span data-ttu-id="143d0-115">Application</span><span class="sxs-lookup"><span data-stu-id="143d0-115">Application</span></span>                            | <span data-ttu-id="143d0-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="143d0-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="143d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="143d0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="143d0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="143d0-118">Optional query parameters</span></span>

<span data-ttu-id="143d0-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="143d0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="143d0-120">Para obter informações gerais, consulte [Parâmetros de Consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="143d0-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="143d0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="143d0-121">Request headers</span></span>

| <span data-ttu-id="143d0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="143d0-122">Name</span></span>      |<span data-ttu-id="143d0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="143d0-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="143d0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="143d0-124">Authorization</span></span> | <span data-ttu-id="143d0-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="143d0-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="143d0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="143d0-126">Request body</span></span>

<span data-ttu-id="143d0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="143d0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="143d0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="143d0-128">Response</span></span>

<span data-ttu-id="143d0-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto tiIndicator](../resources/tiindicator.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="143d0-129">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="143d0-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="143d0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="143d0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="143d0-131">Request</span></span>

<span data-ttu-id="143d0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="143d0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="143d0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="143d0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="c"></a>[<span data-ttu-id="143d0-134">C#</span><span class="sxs-lookup"><span data-stu-id="143d0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="143d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="143d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="143d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="143d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="143d0-137">Java</span><span class="sxs-lookup"><span data-stu-id="143d0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="143d0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="143d0-138">Response</span></span>

<span data-ttu-id="143d0-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="143d0-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="143d0-140">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="143d0-140">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "action": "action-value",
  "activityGroupNames": [
    "activityGroupNames-value"
  ],
  "additionalInformation": "additionalInformation-value",
  "azureTenantId": "azureTenantId-value",
  "confidence": 99,
  "description": "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


