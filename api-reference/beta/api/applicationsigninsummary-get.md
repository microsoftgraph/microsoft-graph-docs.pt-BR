---
title: Obter applicationSignInSummary
description: Recupere as propriedades e os relacionamentos de um objeto **applicationSigninSummary** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f52c24bb1b47e1c8c3302ac3b876ae6983d067d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719008"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="90ef4-103">Obter applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="90ef4-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90ef4-104">Recupere as propriedades e os relacionamentos de um objeto [applicationSigninSummary](../resources/applicationsigninsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="90ef4-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90ef4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="90ef4-105">Permissions</span></span>
<span data-ttu-id="90ef4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="90ef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="90ef4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90ef4-108">Permission type</span></span>      | <span data-ttu-id="90ef4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90ef4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90ef4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90ef4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90ef4-111">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="90ef4-111">Report.Read.All</span></span> |
|<span data-ttu-id="90ef4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90ef4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90ef4-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="90ef4-113">Not supported</span></span>   |
|<span data-ttu-id="90ef4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90ef4-114">Application</span></span> | <span data-ttu-id="90ef4-115">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="90ef4-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="90ef4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90ef4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="90ef4-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="90ef4-117">Function parameters</span></span>

| <span data-ttu-id="90ef4-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="90ef4-118">Parameter</span></span> | <span data-ttu-id="90ef4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ef4-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="90ef4-120">ponto</span><span class="sxs-lookup"><span data-stu-id="90ef4-120">period</span></span> | <span data-ttu-id="90ef4-121">`D7` (Últimos sete dias) ou `D30` (últimos 30 dias); outros valores geram erros.</span><span class="sxs-lookup"><span data-stu-id="90ef4-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="90ef4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90ef4-122">Request headers</span></span>
| <span data-ttu-id="90ef4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="90ef4-123">Name</span></span>      |<span data-ttu-id="90ef4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ef4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90ef4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="90ef4-125">Authorization</span></span> | <span data-ttu-id="90ef4-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="90ef4-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="90ef4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90ef4-127">Request body</span></span>
<span data-ttu-id="90ef4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90ef4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90ef4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ef4-129">Response</span></span>
<span data-ttu-id="90ef4-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [applicationSignInSummary](../resources/applicationsigninsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ef4-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ef4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90ef4-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="90ef4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90ef4-132">Request</span></span>
<span data-ttu-id="90ef4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90ef4-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90ef4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="90ef4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90ef4-135">C#</span><span class="sxs-lookup"><span data-stu-id="90ef4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90ef4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90ef4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90ef4-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="90ef4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="90ef4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ef4-138">Response</span></span>
<span data-ttu-id="90ef4-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90ef4-139">The following is an example of the response.</span></span> 

><span data-ttu-id="90ef4-140">**Observação:** O objeto Response mostrado aqui mmight ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="90ef4-140">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="90ef4-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90ef4-141">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
