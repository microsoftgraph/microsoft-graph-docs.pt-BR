---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 99206c53b6b7c9b609afb1897b6ae0c7e3224e81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451510"
---
# <a name="close-session"></a><span data-ttu-id="bcebe-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="bcebe-103">Close Session</span></span>

<span data-ttu-id="bcebe-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bcebe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bcebe-105">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="bcebe-105">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bcebe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcebe-106">Permissions</span></span>
<span data-ttu-id="bcebe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcebe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcebe-109">Permission type</span></span>      | <span data-ttu-id="bcebe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcebe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcebe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcebe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bcebe-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcebe-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bcebe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcebe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcebe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcebe-114">Not supported.</span></span>    |
|<span data-ttu-id="bcebe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcebe-115">Application</span></span> | <span data-ttu-id="bcebe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcebe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcebe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcebe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="bcebe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcebe-118">Request headers</span></span>
| <span data-ttu-id="bcebe-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bcebe-119">Name</span></span>       | <span data-ttu-id="bcebe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcebe-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bcebe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcebe-121">Authorization</span></span>  | <span data-ttu-id="bcebe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcebe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bcebe-124">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="bcebe-124">workbook-session-id</span></span> | <span data-ttu-id="bcebe-125">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="bcebe-125">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcebe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcebe-126">Request body</span></span>
<span data-ttu-id="bcebe-127">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcebe-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="bcebe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcebe-128">Response</span></span>

<span data-ttu-id="bcebe-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bcebe-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bcebe-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcebe-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bcebe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcebe-131">Request</span></span>
<span data-ttu-id="bcebe-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcebe-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bcebe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcebe-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bcebe-134">C#</span><span class="sxs-lookup"><span data-stu-id="bcebe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcebe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcebe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcebe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcebe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="bcebe-137">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="bcebe-137">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="bcebe-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcebe-138">Response</span></span>
<span data-ttu-id="bcebe-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcebe-139">Here is an example of the response.</span></span> 

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
