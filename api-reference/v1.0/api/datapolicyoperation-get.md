---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13b2668d71dbf4bf1e1a708f46594caeacd7b8f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973384"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="27516-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="27516-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="27516-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27516-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27516-105">Recupere as propriedades de um objeto **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="27516-105">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27516-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="27516-106">Permissions</span></span>
<span data-ttu-id="27516-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27516-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27516-109">Permission type</span></span>      | <span data-ttu-id="27516-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27516-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27516-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27516-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="27516-112">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="27516-112">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="27516-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27516-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="27516-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="27516-114">Not applicable</span></span>  |
|<span data-ttu-id="27516-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27516-115">Application</span></span> | <span data-ttu-id="27516-116">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="27516-116">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="27516-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27516-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="27516-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27516-118">Request headers</span></span>
| <span data-ttu-id="27516-119">Nome</span><span class="sxs-lookup"><span data-stu-id="27516-119">Name</span></span>      |<span data-ttu-id="27516-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="27516-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27516-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="27516-121">Authorization</span></span>  | <span data-ttu-id="27516-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="27516-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="27516-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27516-123">Request body</span></span>
<span data-ttu-id="27516-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27516-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="27516-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="27516-125">Response</span></span>
<span data-ttu-id="27516-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27516-126">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27516-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27516-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27516-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27516-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="27516-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="27516-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="27516-130">C#</span><span class="sxs-lookup"><span data-stu-id="27516-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27516-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27516-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27516-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27516-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27516-133">Java</span><span class="sxs-lookup"><span data-stu-id="27516-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-datapolicyoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27516-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="27516-134">Response</span></span>
><span data-ttu-id="27516-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27516-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "progress": "double-value"
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

