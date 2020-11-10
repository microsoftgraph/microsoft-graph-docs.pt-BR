---
title: Obter workforceIntegration
description: Recupere as propriedades e os relacionamentos do objeto workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 98c30115fabbefd32ae0d82ce3cc1e4f0de5cab5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970727"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="4ec7d-103">Obter workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="4ec7d-103">Get workforceIntegration</span></span>

<span data-ttu-id="4ec7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ec7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ec7d-105">Recupere as propriedades e os relacionamentos de um objeto [workforceintegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="4ec7d-105">Retrieve the properties and relationships of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ec7d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ec7d-106">Permissions</span></span>

<span data-ttu-id="4ec7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ec7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ec7d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ec7d-109">Permission type</span></span>                        | <span data-ttu-id="4ec7d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ec7d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4ec7d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ec7d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ec7d-112">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4ec7d-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="4ec7d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ec7d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ec7d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec7d-114">Not supported.</span></span> |
| <span data-ttu-id="4ec7d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ec7d-115">Application</span></span>                            | <span data-ttu-id="4ec7d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ec7d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ec7d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec7d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ec7d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ec7d-118">Optional query parameters</span></span>

<span data-ttu-id="4ec7d-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ec7d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4ec7d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4ec7d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ec7d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec7d-121">Request headers</span></span>

| <span data-ttu-id="4ec7d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4ec7d-122">Name</span></span>      |<span data-ttu-id="4ec7d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ec7d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ec7d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ec7d-124">Authorization</span></span> | <span data-ttu-id="4ec7d-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4ec7d-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ec7d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec7d-126">Request body</span></span>

<span data-ttu-id="4ec7d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ec7d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ec7d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec7d-128">Response</span></span>

<span data-ttu-id="4ec7d-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [workforceIntegration](../resources/workforceintegration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ec7d-129">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ec7d-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4ec7d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ec7d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ec7d-131">Request</span></span>

<span data-ttu-id="4ec7d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ec7d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ec7d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec7d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="c"></a>[<span data-ttu-id="4ec7d-134">C#</span><span class="sxs-lookup"><span data-stu-id="4ec7d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ec7d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ec7d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ec7d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ec7d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ec7d-137">Java</span><span class="sxs-lookup"><span data-stu-id="4ec7d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ec7d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ec7d-138">Response</span></span>

<span data-ttu-id="4ec7d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ec7d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4ec7d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ec7d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supports": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


