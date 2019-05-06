---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 749f9e62536949e4e74077640076337f7d8a5263
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591031"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="d26da-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d26da-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="d26da-104">Recupere as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="d26da-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d26da-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d26da-105">Permissions</span></span>
<span data-ttu-id="d26da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d26da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d26da-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d26da-108">Permission type</span></span>      | <span data-ttu-id="d26da-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d26da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d26da-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d26da-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d26da-111">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="d26da-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="d26da-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d26da-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d26da-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="d26da-113">Not applicable</span></span>  |
|<span data-ttu-id="d26da-114">Application</span><span class="sxs-lookup"><span data-stu-id="d26da-114">Application</span></span> | <span data-ttu-id="d26da-115">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="d26da-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d26da-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d26da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d26da-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d26da-117">Request headers</span></span>
| <span data-ttu-id="d26da-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d26da-118">Name</span></span>      |<span data-ttu-id="d26da-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d26da-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d26da-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d26da-120">Authorization</span></span>  | <span data-ttu-id="d26da-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d26da-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d26da-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d26da-122">Request body</span></span>
<span data-ttu-id="d26da-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d26da-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d26da-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="d26da-124">Response</span></span>
<span data-ttu-id="d26da-125">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d26da-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d26da-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d26da-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d26da-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d26da-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="d26da-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d26da-128">Response</span></span>
<span data-ttu-id="d26da-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d26da-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d26da-131">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d26da-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d26da-132">Basic</span><span class="sxs-lookup"><span data-stu-id="d26da-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d26da-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d26da-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
