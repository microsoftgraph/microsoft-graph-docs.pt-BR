---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c96cf23c137c0b518d0b9819a52a23631b1cd488
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046990"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="ed891-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="ed891-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="ed891-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed891-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed891-105">Recupere as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="ed891-105">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed891-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed891-106">Permissions</span></span>
<span data-ttu-id="ed891-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed891-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed891-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed891-109">Permission type</span></span>      | <span data-ttu-id="ed891-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed891-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed891-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed891-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ed891-112">User.Export.All e User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed891-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="ed891-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed891-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ed891-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="ed891-114">Not applicable</span></span>  |
|<span data-ttu-id="ed891-115">Application</span><span class="sxs-lookup"><span data-stu-id="ed891-115">Application</span></span> | <span data-ttu-id="ed891-116">User.Export.All e User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed891-116">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ed891-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed891-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ed891-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed891-118">Request headers</span></span>
| <span data-ttu-id="ed891-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ed891-119">Name</span></span>      |<span data-ttu-id="ed891-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed891-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed891-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed891-121">Authorization</span></span>  | <span data-ttu-id="ed891-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ed891-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed891-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed891-123">Request body</span></span>
<span data-ttu-id="ed891-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed891-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ed891-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed891-125">Response</span></span>
<span data-ttu-id="ed891-126">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed891-126">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed891-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed891-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed891-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed891-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ed891-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed891-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="ed891-130">C#</span><span class="sxs-lookup"><span data-stu-id="ed891-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed891-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed891-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed891-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed891-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed891-133">Java</span><span class="sxs-lookup"><span data-stu-id="ed891-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-datapolicyoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ed891-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed891-134">Response</span></span>
<span data-ttu-id="ed891-135">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ed891-135">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value",
  "progress": "double"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


