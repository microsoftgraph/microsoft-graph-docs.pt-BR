---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6979d9f17a7a67e93da32fcc97036304e1cc6dc
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124263"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="1c46d-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1c46d-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="1c46d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c46d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c46d-105">Recupere as propriedades de um objeto **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="1c46d-105">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c46d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c46d-106">Permissions</span></span>
<span data-ttu-id="1c46d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c46d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c46d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c46d-109">Permission type</span></span>      | <span data-ttu-id="1c46d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c46d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c46d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c46d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1c46d-112">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="1c46d-112">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="1c46d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c46d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1c46d-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="1c46d-114">Not applicable</span></span>  |
|<span data-ttu-id="1c46d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c46d-115">Application</span></span> | <span data-ttu-id="1c46d-116">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="1c46d-116">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1c46d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c46d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1c46d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c46d-118">Request headers</span></span>
| <span data-ttu-id="1c46d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1c46d-119">Name</span></span>      |<span data-ttu-id="1c46d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c46d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c46d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c46d-121">Authorization</span></span>  | <span data-ttu-id="1c46d-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1c46d-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c46d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c46d-123">Request body</span></span>
<span data-ttu-id="1c46d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c46d-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1c46d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c46d-125">Response</span></span>
<span data-ttu-id="1c46d-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c46d-126">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c46d-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c46d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c46d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c46d-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1c46d-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c46d-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="1c46d-130">C#</span><span class="sxs-lookup"><span data-stu-id="1c46d-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c46d-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c46d-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c46d-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c46d-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c46d-133">Java</span><span class="sxs-lookup"><span data-stu-id="1c46d-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-datapolicyoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c46d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c46d-134">Response</span></span>
><span data-ttu-id="1c46d-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c46d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
