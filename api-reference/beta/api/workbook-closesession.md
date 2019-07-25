---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6b172fcf56f82404104fd16a780191edc5337c20
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866632"
---
# <a name="close-session"></a><span data-ttu-id="b06fa-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="b06fa-103">Close Session</span></span>

<span data-ttu-id="b06fa-104">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="b06fa-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b06fa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b06fa-105">Permissions</span></span>
<span data-ttu-id="b06fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b06fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b06fa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b06fa-108">Permission type</span></span>      | <span data-ttu-id="b06fa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b06fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b06fa-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b06fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b06fa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b06fa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b06fa-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b06fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b06fa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b06fa-113">Not supported.</span></span>    |
|<span data-ttu-id="b06fa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b06fa-114">Application</span></span> | <span data-ttu-id="b06fa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b06fa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b06fa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b06fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="b06fa-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b06fa-117">Request headers</span></span>
| <span data-ttu-id="b06fa-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b06fa-118">Name</span></span>       | <span data-ttu-id="b06fa-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b06fa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b06fa-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b06fa-120">Authorization</span></span>  | <span data-ttu-id="b06fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b06fa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b06fa-123">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="b06fa-123">workbook-session-id</span></span> | <span data-ttu-id="b06fa-124">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="b06fa-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="b06fa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b06fa-125">Request body</span></span>
<span data-ttu-id="b06fa-126">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b06fa-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="b06fa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b06fa-127">Response</span></span>

<span data-ttu-id="b06fa-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b06fa-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b06fa-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b06fa-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b06fa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b06fa-130">Request</span></span>
<span data-ttu-id="b06fa-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b06fa-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b06fa-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b06fa-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b06fa-133">C#</span><span class="sxs-lookup"><span data-stu-id="b06fa-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b06fa-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b06fa-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b06fa-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b06fa-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b06fa-136">Java</span><span class="sxs-lookup"><span data-stu-id="b06fa-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/close-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="b06fa-137">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="b06fa-137">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="b06fa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b06fa-138">Response</span></span>
<span data-ttu-id="b06fa-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b06fa-139">Here is an example of the response.</span></span> 

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
