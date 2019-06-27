---
title: Obter applicationSignInDetailedSummary
description: Recupere as propriedades e os relacionamentos de um objeto applicationSignInDetailSummary.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96b2e9bf87dd953ea6c53ae2d19c37c294425e35
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258397"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="6b289-103">Obter applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="6b289-103">Get applicationSignInDetailedSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b289-104">Recupere as propriedades e os relacionamentos de um objeto [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="6b289-104">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b289-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b289-105">Permissions</span></span>
<span data-ttu-id="6b289-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="6b289-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b289-108">Permission type</span></span>                        | <span data-ttu-id="6b289-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b289-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b289-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b289-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b289-111">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="6b289-111">Report.Read.All</span></span> |
|<span data-ttu-id="6b289-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b289-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b289-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b289-113">Not supported.</span></span> |
|<span data-ttu-id="6b289-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b289-114">Application</span></span>                            | <span data-ttu-id="6b289-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b289-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b289-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b289-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b289-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b289-117">Optional query parameters</span></span>

<span data-ttu-id="6b289-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6b289-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b289-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b289-119">Request headers</span></span>

| <span data-ttu-id="6b289-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6b289-120">Name</span></span>      |<span data-ttu-id="6b289-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b289-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b289-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b289-122">Authorization</span></span> | <span data-ttu-id="6b289-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6b289-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b289-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b289-124">Request body</span></span>
<span data-ttu-id="6b289-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b289-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b289-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b289-126">Response</span></span>
<span data-ttu-id="6b289-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b289-127">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b289-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b289-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b289-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b289-129">Request</span></span>
<span data-ttu-id="6b289-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b289-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/<id>
```

### <a name="response"></a><span data-ttu-id="6b289-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b289-131">Response</span></span>
<span data-ttu-id="6b289-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b289-132">The following is an example of the response.</span></span> 

><span data-ttu-id="6b289-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b289-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6b289-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6b289-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6b289-136">C#</span><span class="sxs-lookup"><span data-stu-id="6b289-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_applicationsignindetailedsummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b289-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="6b289-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_applicationsignindetailedsummary-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6b289-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6b289-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_applicationsignindetailedsummary-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/applicationsignindetailedsummary-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/applicationsignindetailedsummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/applicationsignindetailedsummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
