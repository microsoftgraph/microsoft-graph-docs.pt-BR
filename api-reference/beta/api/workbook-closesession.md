---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26570479e6439e6eb1fd8b58efb9a96a1a60b123
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269857"
---
# <a name="close-session"></a><span data-ttu-id="59e1c-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="59e1c-103">Close Session</span></span>

<span data-ttu-id="59e1c-104">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="59e1c-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="59e1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="59e1c-105">Permissions</span></span>
<span data-ttu-id="59e1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59e1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59e1c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59e1c-108">Permission type</span></span>      | <span data-ttu-id="59e1c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59e1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59e1c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59e1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59e1c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59e1c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59e1c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59e1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59e1c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59e1c-113">Not supported.</span></span>    |
|<span data-ttu-id="59e1c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59e1c-114">Application</span></span> | <span data-ttu-id="59e1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59e1c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59e1c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59e1c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="59e1c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59e1c-117">Request headers</span></span>
| <span data-ttu-id="59e1c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="59e1c-118">Name</span></span>       | <span data-ttu-id="59e1c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="59e1c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59e1c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="59e1c-120">Authorization</span></span>  | <span data-ttu-id="59e1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59e1c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59e1c-123">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="59e1c-123">workbook-session-id</span></span> | <span data-ttu-id="59e1c-124">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="59e1c-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="59e1c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59e1c-125">Request body</span></span>
<span data-ttu-id="59e1c-126">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59e1c-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="59e1c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="59e1c-127">Response</span></span>

<span data-ttu-id="59e1c-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="59e1c-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="59e1c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59e1c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59e1c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59e1c-130">Request</span></span>
<span data-ttu-id="59e1c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59e1c-131">Here is an example of the request.</span></span>
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

<span data-ttu-id="59e1c-132">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="59e1c-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="59e1c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="59e1c-133">Response</span></span>
<span data-ttu-id="59e1c-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59e1c-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="59e1c-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="59e1c-135">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59e1c-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="59e1c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/close_excel_session-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="59e1c-137">C#</span><span class="sxs-lookup"><span data-stu-id="59e1c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/close_excel_session-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="59e1c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="59e1c-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/close_excel_session-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
