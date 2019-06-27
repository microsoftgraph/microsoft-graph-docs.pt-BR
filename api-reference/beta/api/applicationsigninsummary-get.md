---
title: Obter applicationSignInSummary
description: Recupere as propriedades e os relacionamentos de um objeto **applicationSigninSummary** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb9dfa4f57226ed846fcf7e7b6668214ad4be7ca
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258391"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="e2b25-103">Obter applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="e2b25-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2b25-104">Recupere as propriedades e os relacionamentos de um objeto [applicationSigninSummary](../resources/applicationsigninsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e2b25-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2b25-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2b25-105">Permissions</span></span>
<span data-ttu-id="e2b25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e2b25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="e2b25-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2b25-108">Permission type</span></span>      | <span data-ttu-id="e2b25-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2b25-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2b25-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2b25-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2b25-111">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="e2b25-111">Report.Read.All</span></span> |
|<span data-ttu-id="e2b25-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2b25-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2b25-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e2b25-113">Not supported</span></span>   |
|<span data-ttu-id="e2b25-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2b25-114">Application</span></span> | <span data-ttu-id="e2b25-115">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="e2b25-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e2b25-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2b25-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="e2b25-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e2b25-117">Function parameters</span></span>

| <span data-ttu-id="e2b25-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e2b25-118">Parameter</span></span> | <span data-ttu-id="e2b25-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2b25-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="e2b25-120">ponto</span><span class="sxs-lookup"><span data-stu-id="e2b25-120">period</span></span> | <span data-ttu-id="e2b25-121">`D7` (Últimos sete dias) ou `D30` (últimos 30 dias); outros valores geram erros.</span><span class="sxs-lookup"><span data-stu-id="e2b25-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e2b25-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b25-122">Request headers</span></span>
| <span data-ttu-id="e2b25-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e2b25-123">Name</span></span>      |<span data-ttu-id="e2b25-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2b25-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2b25-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2b25-125">Authorization</span></span> | <span data-ttu-id="e2b25-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e2b25-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2b25-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b25-127">Request body</span></span>
<span data-ttu-id="e2b25-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e2b25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2b25-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2b25-129">Response</span></span>
<span data-ttu-id="e2b25-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [applicationSignInSummary](../resources/applicationsigninsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2b25-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2b25-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2b25-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2b25-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b25-132">Request</span></span>
<span data-ttu-id="e2b25-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2b25-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
### <a name="response"></a><span data-ttu-id="e2b25-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2b25-134">Response</span></span>
<span data-ttu-id="e2b25-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e2b25-135">The following is an example of the response.</span></span> 

><span data-ttu-id="e2b25-136">**Observação:** O objeto Response mostrado aqui mmight ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="e2b25-136">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="e2b25-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2b25-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "successfulSignInCount": 99,
  "failedSignInCount": 99,
  "successPercentage": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e2b25-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e2b25-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e2b25-139">C#</span><span class="sxs-lookup"><span data-stu-id="e2b25-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2b25-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="e2b25-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e2b25-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e2b25-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
