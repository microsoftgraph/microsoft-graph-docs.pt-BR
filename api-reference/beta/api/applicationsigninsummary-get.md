---
title: Obter applicationSignInSummary
description: Recupere as propriedades e os relacionamentos de um objeto **applicationSigninSummary** .
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c7b085b8142c8f2bd2a2a0b0f502178a7179a398
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107042"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="b1754-103">Obter applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="b1754-103">Get applicationSignInSummary</span></span>

<span data-ttu-id="b1754-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1754-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1754-105">Recupere as propriedades e os relacionamentos de um objeto [applicationSigninSummary](../resources/applicationsigninsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b1754-105">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1754-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1754-106">Permissions</span></span>
<span data-ttu-id="b1754-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="b1754-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1754-109">Permission type</span></span>      | <span data-ttu-id="b1754-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1754-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1754-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1754-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b1754-112">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="b1754-112">Report.Read.All</span></span> |
|<span data-ttu-id="b1754-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1754-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1754-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b1754-114">Not supported</span></span>   |
|<span data-ttu-id="b1754-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1754-115">Application</span></span> | <span data-ttu-id="b1754-116">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="b1754-116">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b1754-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1754-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="b1754-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b1754-118">Function parameters</span></span>

| <span data-ttu-id="b1754-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b1754-119">Parameter</span></span> | <span data-ttu-id="b1754-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1754-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b1754-121">ponto</span><span class="sxs-lookup"><span data-stu-id="b1754-121">period</span></span> | <span data-ttu-id="b1754-122">`D7` (Últimos sete dias) ou `D30` (últimos 30 dias); outros valores geram erros.</span><span class="sxs-lookup"><span data-stu-id="b1754-122">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b1754-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1754-123">Request headers</span></span>
| <span data-ttu-id="b1754-124">Nome</span><span class="sxs-lookup"><span data-stu-id="b1754-124">Name</span></span>      |<span data-ttu-id="b1754-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1754-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b1754-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1754-126">Authorization</span></span> | <span data-ttu-id="b1754-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b1754-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1754-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1754-128">Request body</span></span>
<span data-ttu-id="b1754-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1754-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1754-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1754-130">Response</span></span>
<span data-ttu-id="b1754-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [applicationSignInSummary](../resources/applicationsigninsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1754-131">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1754-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1754-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1754-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1754-133">Request</span></span>
<span data-ttu-id="b1754-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1754-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1754-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1754-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="b1754-136">C#</span><span class="sxs-lookup"><span data-stu-id="b1754-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1754-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1754-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1754-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1754-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b1754-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1754-139">Response</span></span>
<span data-ttu-id="b1754-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1754-140">The following is an example of the response.</span></span> 

><span data-ttu-id="b1754-141">**Observação:** O objeto Response mostrado aqui mmight ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="b1754-141">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="b1754-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1754-142">All the properties will be returned from an actual call.</span></span>
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
