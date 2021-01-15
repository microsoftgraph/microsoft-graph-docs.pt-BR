---
title: Obter continuousAccessEvaluationPolicy
description: Leia as propriedades de um objeto continuousAccessEvaluationPolicy.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8dcafa080167facb1a692af8634fb6d1f4f345b5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872650"
---
# <a name="get-continuousaccessevaluationpolicy"></a><span data-ttu-id="91fca-103">Obter continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="91fca-103">Get continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="91fca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91fca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91fca-105">Leia as propriedades e as relações de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91fca-105">Read the properties and relationships of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91fca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="91fca-106">Permissions</span></span>
<span data-ttu-id="91fca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91fca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91fca-109">Permission type</span></span>|<span data-ttu-id="91fca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91fca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91fca-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91fca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91fca-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="91fca-112">Policy.Read.All</span></span> |
|<span data-ttu-id="91fca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91fca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91fca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91fca-114">Not supported.</span></span> |
|<span data-ttu-id="91fca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91fca-115">Application</span></span>                            | <span data-ttu-id="91fca-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="91fca-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91fca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91fca-117">HTTP request</span></span>

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91fca-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91fca-118">Optional query parameters</span></span>
<span data-ttu-id="91fca-119">Esse método dá suporte ao parâmetro de consulta OData "$select" para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="91fca-119">This method supports the '$select' OData query parameter to help customize the response.</span></span> <span data-ttu-id="91fca-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="91fca-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="91fca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91fca-121">Request headers</span></span>
|<span data-ttu-id="91fca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="91fca-122">Name</span></span>|<span data-ttu-id="91fca-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="91fca-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="91fca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="91fca-124">Authorization</span></span>|<span data-ttu-id="91fca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91fca-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91fca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91fca-127">Request body</span></span>
<span data-ttu-id="91fca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91fca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91fca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="91fca-129">Response</span></span>

<span data-ttu-id="91fca-130">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91fca-130">If successful, this method returns a `200 OK` response code and a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91fca-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="91fca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91fca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91fca-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="91fca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="91fca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```
# <a name="c"></a>[<span data-ttu-id="91fca-134">C#</span><span class="sxs-lookup"><span data-stu-id="91fca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91fca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91fca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91fca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91fca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91fca-137">Java</span><span class="sxs-lookup"><span data-stu-id="91fca-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-continuousaccessevaluationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="91fca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="91fca-138">Response</span></span>

<span data-ttu-id="91fca-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91fca-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
