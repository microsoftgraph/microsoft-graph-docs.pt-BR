---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 08cfbf935a1a37be83349d2d75631bc8767ec8d8
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123682"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="b250e-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b250e-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="b250e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b250e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b250e-105">Recupere as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="b250e-105">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b250e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b250e-106">Permissions</span></span>
<span data-ttu-id="b250e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b250e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b250e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b250e-109">Permission type</span></span>      | <span data-ttu-id="b250e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b250e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b250e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b250e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b250e-112">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="b250e-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="b250e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b250e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b250e-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="b250e-114">Not applicable</span></span>  |
|<span data-ttu-id="b250e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b250e-115">Application</span></span> | <span data-ttu-id="b250e-116">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="b250e-116">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b250e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b250e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b250e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b250e-118">Request headers</span></span>
| <span data-ttu-id="b250e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b250e-119">Name</span></span>      |<span data-ttu-id="b250e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b250e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b250e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b250e-121">Authorization</span></span>  | <span data-ttu-id="b250e-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b250e-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b250e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b250e-123">Request body</span></span>
<span data-ttu-id="b250e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b250e-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b250e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b250e-125">Response</span></span>
<span data-ttu-id="b250e-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b250e-126">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b250e-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b250e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b250e-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b250e-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b250e-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="b250e-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="b250e-130">C#</span><span class="sxs-lookup"><span data-stu-id="b250e-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b250e-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b250e-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b250e-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b250e-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b250e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b250e-133">Response</span></span>
<span data-ttu-id="b250e-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b250e-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
