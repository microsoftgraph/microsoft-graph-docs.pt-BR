---
title: Obter applicationSignInDetailedSummary
description: Recupere as propriedades e os relacionamentos de um objeto applicationSignInDetailSummary.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 429047008353c658349498b6cafda59942fc3930
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945414"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="7fdd7-103">Obter applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="7fdd7-103">Get applicationSignInDetailedSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fdd7-104">Recupere as propriedades e os relacionamentos de um objeto [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7fdd7-104">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fdd7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fdd7-105">Permissions</span></span>
<span data-ttu-id="7fdd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fdd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="7fdd7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fdd7-108">Permission type</span></span>                        | <span data-ttu-id="7fdd7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fdd7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fdd7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fdd7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fdd7-111">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="7fdd7-111">Report.Read.All</span></span> |
|<span data-ttu-id="7fdd7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fdd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fdd7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fdd7-113">Not supported.</span></span> |
|<span data-ttu-id="7fdd7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fdd7-114">Application</span></span>                            | <span data-ttu-id="7fdd7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fdd7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fdd7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fdd7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fdd7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7fdd7-117">Optional query parameters</span></span>

<span data-ttu-id="7fdd7-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7fdd7-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fdd7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdd7-119">Request headers</span></span>

| <span data-ttu-id="7fdd7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7fdd7-120">Name</span></span>      |<span data-ttu-id="7fdd7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fdd7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7fdd7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fdd7-122">Authorization</span></span> | <span data-ttu-id="7fdd7-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7fdd7-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fdd7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdd7-124">Request body</span></span>
<span data-ttu-id="7fdd7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fdd7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fdd7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fdd7-126">Response</span></span>
<span data-ttu-id="7fdd7-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fdd7-127">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fdd7-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fdd7-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fdd7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fdd7-129">Request</span></span>
<span data-ttu-id="7fdd7-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fdd7-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7fdd7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fdd7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7fdd7-132">C#</span><span class="sxs-lookup"><span data-stu-id="7fdd7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7fdd7-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="7fdd7-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7fdd7-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7fdd7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7fdd7-135">Java</span><span class="sxs-lookup"><span data-stu-id="7fdd7-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsignindetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fdd7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fdd7-136">Response</span></span>
<span data-ttu-id="7fdd7-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fdd7-137">The following is an example of the response.</span></span> 

><span data-ttu-id="7fdd7-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fdd7-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
