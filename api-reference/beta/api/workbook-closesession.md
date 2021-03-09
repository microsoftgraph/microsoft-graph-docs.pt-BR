---
title: Fechar Sessão
description: 'Use essa API para fechar uma sessão de workbook existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 82093330409b856f2c893436279260f273c02b5a
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578826"
---
# <a name="close-session"></a><span data-ttu-id="75ac7-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="75ac7-103">Close Session</span></span>

<span data-ttu-id="75ac7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75ac7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75ac7-105">Use essa API para fechar uma sessão de workbook existente.</span><span class="sxs-lookup"><span data-stu-id="75ac7-105">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="75ac7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="75ac7-106">Permissions</span></span>
<span data-ttu-id="75ac7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75ac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75ac7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75ac7-109">Permission type</span></span>      | <span data-ttu-id="75ac7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75ac7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75ac7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75ac7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="75ac7-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75ac7-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75ac7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75ac7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75ac7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75ac7-114">Not supported.</span></span>    |
|<span data-ttu-id="75ac7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75ac7-115">Application</span></span> | <span data-ttu-id="75ac7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75ac7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75ac7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75ac7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/closeSession
POST /me/drive/root:/{item-path}:/workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="75ac7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75ac7-118">Request headers</span></span>
| <span data-ttu-id="75ac7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="75ac7-119">Name</span></span>       | <span data-ttu-id="75ac7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="75ac7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75ac7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="75ac7-121">Authorization</span></span>  | <span data-ttu-id="75ac7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75ac7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75ac7-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="75ac7-124">workbook-session-id</span></span> | <span data-ttu-id="75ac7-125">ID da sessão de workbook a ser fechada</span><span class="sxs-lookup"><span data-stu-id="75ac7-125">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="75ac7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75ac7-126">Request body</span></span>
<span data-ttu-id="75ac7-127">Essa API não exige nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="75ac7-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="75ac7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="75ac7-128">Response</span></span>

<span data-ttu-id="75ac7-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="75ac7-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="75ac7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75ac7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75ac7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75ac7-131">Request</span></span>
<span data-ttu-id="75ac7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75ac7-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75ac7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="75ac7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="c"></a>[<span data-ttu-id="75ac7-134">C#</span><span class="sxs-lookup"><span data-stu-id="75ac7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75ac7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75ac7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75ac7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75ac7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75ac7-137">Java</span><span class="sxs-lookup"><span data-stu-id="75ac7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/close-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="75ac7-138">Observe que o header workbook-session-id é necessário.</span><span class="sxs-lookup"><span data-stu-id="75ac7-138">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="75ac7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="75ac7-139">Response</span></span>
<span data-ttu-id="75ac7-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75ac7-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


