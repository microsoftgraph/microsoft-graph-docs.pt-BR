---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01cf28480b8b0d8f54bba08fb74e46a633000b2f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276374"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="981ea-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="981ea-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="981ea-104">Recupere as propriedades de um objeto **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="981ea-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="981ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="981ea-105">Permissions</span></span>
<span data-ttu-id="981ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="981ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="981ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="981ea-108">Permission type</span></span>      | <span data-ttu-id="981ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="981ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="981ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="981ea-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="981ea-111">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="981ea-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="981ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="981ea-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="981ea-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="981ea-113">Not applicable</span></span>  |
|<span data-ttu-id="981ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="981ea-114">Application</span></span> | <span data-ttu-id="981ea-115">User. Export. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="981ea-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="981ea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="981ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="981ea-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="981ea-117">Request headers</span></span>
| <span data-ttu-id="981ea-118">Nome</span><span class="sxs-lookup"><span data-stu-id="981ea-118">Name</span></span>      |<span data-ttu-id="981ea-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="981ea-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="981ea-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="981ea-120">Authorization</span></span>  | <span data-ttu-id="981ea-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="981ea-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="981ea-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="981ea-122">Request body</span></span>
<span data-ttu-id="981ea-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="981ea-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="981ea-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="981ea-124">Response</span></span>
<span data-ttu-id="981ea-125">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="981ea-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="981ea-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="981ea-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="981ea-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="981ea-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="981ea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="981ea-128">Response</span></span>
><span data-ttu-id="981ea-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="981ea-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="981ea-131">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="981ea-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="981ea-132">C#</span><span class="sxs-lookup"><span data-stu-id="981ea-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="981ea-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="981ea-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="981ea-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="981ea-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
