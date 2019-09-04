---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f230ec987ebb574d741a25f388feef79e221ec3
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718293"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="8bc90-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="8bc90-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="8bc90-104">Recupere as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="8bc90-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bc90-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bc90-105">Permissions</span></span>
<span data-ttu-id="8bc90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bc90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bc90-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bc90-108">Permission type</span></span>      | <span data-ttu-id="8bc90-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bc90-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bc90-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bc90-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8bc90-111">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="8bc90-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="8bc90-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bc90-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8bc90-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="8bc90-113">Not applicable</span></span>  |
|<span data-ttu-id="8bc90-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bc90-114">Application</span></span> | <span data-ttu-id="8bc90-115">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="8bc90-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8bc90-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bc90-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bc90-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc90-117">Request headers</span></span>
| <span data-ttu-id="8bc90-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8bc90-118">Name</span></span>      |<span data-ttu-id="8bc90-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bc90-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8bc90-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bc90-120">Authorization</span></span>  | <span data-ttu-id="8bc90-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8bc90-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bc90-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc90-122">Request body</span></span>
<span data-ttu-id="8bc90-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8bc90-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8bc90-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bc90-124">Response</span></span>
<span data-ttu-id="8bc90-125">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bc90-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8bc90-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bc90-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bc90-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc90-127">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8bc90-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bc90-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bc90-129">C#</span><span class="sxs-lookup"><span data-stu-id="8bc90-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bc90-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bc90-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bc90-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8bc90-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8bc90-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bc90-132">Response</span></span>
<span data-ttu-id="8bc90-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bc90-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
