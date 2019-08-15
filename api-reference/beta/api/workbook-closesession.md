---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a58176678a723e672e3683c2b6a1d4ef85726973
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421747"
---
# <a name="close-session"></a><span data-ttu-id="b71a1-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="b71a1-103">Close Session</span></span>

<span data-ttu-id="b71a1-104">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="b71a1-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b71a1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b71a1-105">Permissions</span></span>
<span data-ttu-id="b71a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b71a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b71a1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b71a1-108">Permission type</span></span>      | <span data-ttu-id="b71a1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b71a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b71a1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b71a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b71a1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b71a1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b71a1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b71a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b71a1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b71a1-113">Not supported.</span></span>    |
|<span data-ttu-id="b71a1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b71a1-114">Application</span></span> | <span data-ttu-id="b71a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b71a1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b71a1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b71a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="b71a1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b71a1-117">Request headers</span></span>
| <span data-ttu-id="b71a1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b71a1-118">Name</span></span>       | <span data-ttu-id="b71a1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b71a1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b71a1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b71a1-120">Authorization</span></span>  | <span data-ttu-id="b71a1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b71a1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b71a1-123">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="b71a1-123">workbook-session-id</span></span> | <span data-ttu-id="b71a1-124">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="b71a1-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="b71a1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b71a1-125">Request body</span></span>
<span data-ttu-id="b71a1-126">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b71a1-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="b71a1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b71a1-127">Response</span></span>

<span data-ttu-id="b71a1-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b71a1-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b71a1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b71a1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b71a1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b71a1-130">Request</span></span>
<span data-ttu-id="b71a1-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b71a1-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b71a1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b71a1-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b71a1-133">C#</span><span class="sxs-lookup"><span data-stu-id="b71a1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b71a1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b71a1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b71a1-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b71a1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="b71a1-136">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="b71a1-136">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="b71a1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b71a1-137">Response</span></span>
<span data-ttu-id="b71a1-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b71a1-138">Here is an example of the response.</span></span> 

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
