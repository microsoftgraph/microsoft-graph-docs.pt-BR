---
title: Obter applicationSignInDetailedSummary
description: Recupere as propriedades e os relacionamentos de um objeto applicationSignInDetailSummary.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ae9990b2008e091ca5c821adf360cf8c552fd6d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961810"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="5f559-103">Obter applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="5f559-103">Get applicationSignInDetailedSummary</span></span>

<span data-ttu-id="5f559-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f559-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f559-105">Recupere as propriedades e os relacionamentos de um objeto [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5f559-105">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f559-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f559-106">Permissions</span></span>
<span data-ttu-id="5f559-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="5f559-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f559-109">Permission type</span></span>                        | <span data-ttu-id="5f559-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f559-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f559-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f559-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f559-112">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="5f559-112">Report.Read.All</span></span> |
|<span data-ttu-id="5f559-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f559-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f559-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f559-114">Not supported.</span></span> |
|<span data-ttu-id="5f559-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f559-115">Application</span></span>                            | <span data-ttu-id="5f559-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f559-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f559-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f559-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f559-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f559-118">Optional query parameters</span></span>

<span data-ttu-id="5f559-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f559-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f559-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f559-120">Request headers</span></span>

| <span data-ttu-id="5f559-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5f559-121">Name</span></span>      |<span data-ttu-id="5f559-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f559-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f559-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f559-123">Authorization</span></span> | <span data-ttu-id="5f559-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5f559-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f559-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f559-125">Request body</span></span>
<span data-ttu-id="5f559-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f559-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f559-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f559-127">Response</span></span>
<span data-ttu-id="5f559-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f559-128">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f559-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f559-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f559-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f559-130">Request</span></span>
<span data-ttu-id="5f559-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f559-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f559-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f559-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{id}
```
# <a name="c"></a>[<span data-ttu-id="5f559-133">C#</span><span class="sxs-lookup"><span data-stu-id="5f559-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f559-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f559-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f559-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f559-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f559-136">Java</span><span class="sxs-lookup"><span data-stu-id="5f559-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsignindetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f559-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f559-137">Response</span></span>
<span data-ttu-id="5f559-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f559-138">The following is an example of the response.</span></span> 

><span data-ttu-id="5f559-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f559-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 295

{
  "id": "id-value",
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "status": {
    "errorCode": 99,
    "failureReason": "failureReason-value",
    "additionalDetails": "additionalDetails-value"
  },
  "signInCount": 99,
  "aggregatedEventDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


