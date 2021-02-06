---
title: Obter onPremisesAgent
description: Recupere as propriedades e os relacionamentos de um objeto onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f91b5023d4b45d5ea097e6b09ba9b38eef88561c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136511"
---
# <a name="get-onpremisesagent"></a><span data-ttu-id="18648-103">Obter onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="18648-103">Get onPremisesAgent</span></span>

<span data-ttu-id="18648-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18648-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18648-105">Recupere as propriedades e os relacionamentos de um [objeto onPremisesAgent.](../resources/onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="18648-105">Retrieve the properties and relationships of an [onPremisesAgent](../resources/onpremisesagent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18648-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="18648-106">Permissions</span></span>

<span data-ttu-id="18648-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18648-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18648-109">Permission type</span></span>                        | <span data-ttu-id="18648-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18648-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="18648-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18648-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18648-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18648-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="18648-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18648-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18648-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18648-114">Not supported.</span></span> |
| <span data-ttu-id="18648-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18648-115">Application</span></span>                            | <span data-ttu-id="18648-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18648-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18648-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18648-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/?$expand=agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18648-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="18648-118">Optional query parameters</span></span>

<span data-ttu-id="18648-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="18648-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18648-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18648-120">Request headers</span></span>

| <span data-ttu-id="18648-121">Nome</span><span class="sxs-lookup"><span data-stu-id="18648-121">Name</span></span>      |<span data-ttu-id="18648-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="18648-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="18648-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18648-123">Authorization</span></span> | <span data-ttu-id="18648-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="18648-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="18648-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18648-125">Request body</span></span>

<span data-ttu-id="18648-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18648-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18648-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="18648-127">Response</span></span>

<span data-ttu-id="18648-128">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [onPremisesAgent](../resources/onpremisesagent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18648-128">If successful, this method returns a `200 OK` response code and an [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18648-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="18648-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18648-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18648-130">Request</span></span>

<span data-ttu-id="18648-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18648-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18648-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="18648-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="18648-133">C#</span><span class="sxs-lookup"><span data-stu-id="18648-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisesagent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18648-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18648-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18648-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18648-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18648-136">Java</span><span class="sxs-lookup"><span data-stu-id="18648-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onpremisesagent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18648-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="18648-137">Response</span></span>

<span data-ttu-id="18648-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18648-138">The following is an example of the response.</span></span>

> <span data-ttu-id="18648-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18648-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
    "status": "Active",
    "machineName": "server1.local1.contoso.com",
    "externalIp": "153.69.23.122",
    "agentGroups": [
         {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1"
         }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



