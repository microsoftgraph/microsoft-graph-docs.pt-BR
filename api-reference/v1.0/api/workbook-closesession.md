---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bdff7e46f494527e12bbc1bec3262629120510ed
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278642"
---
# <a name="close-session"></a><span data-ttu-id="bc734-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="bc734-103">Close Session</span></span>

<span data-ttu-id="bc734-104">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="bc734-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bc734-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc734-105">Permissions</span></span>
<span data-ttu-id="bc734-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc734-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc734-108">Permission type</span></span>      | <span data-ttu-id="bc734-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc734-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc734-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc734-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc734-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc734-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc734-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc734-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc734-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc734-113">Not supported.</span></span>    |
|<span data-ttu-id="bc734-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc734-114">Application</span></span> | <span data-ttu-id="bc734-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc734-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc734-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc734-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="bc734-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc734-117">Request headers</span></span>
| <span data-ttu-id="bc734-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bc734-118">Name</span></span>       | <span data-ttu-id="bc734-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc734-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc734-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc734-120">Authorization</span></span>  | <span data-ttu-id="bc734-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc734-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="bc734-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc734-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc734-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bc734-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="bc734-126">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="bc734-126">workbook-session-id</span></span> | <span data-ttu-id="bc734-127">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="bc734-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc734-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc734-128">Request body</span></span>
<span data-ttu-id="bc734-129">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc734-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="bc734-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc734-130">Response</span></span>

<span data-ttu-id="bc734-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bc734-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bc734-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc734-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc734-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc734-133">Request</span></span>
<span data-ttu-id="bc734-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc734-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="bc734-135">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="bc734-135">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="bc734-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc734-136">Response</span></span>
<span data-ttu-id="bc734-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc734-137">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bc734-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bc734-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bc734-139">C#</span><span class="sxs-lookup"><span data-stu-id="bc734-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/close_excel_session-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc734-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="bc734-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/close_excel_session-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bc734-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bc734-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/close_excel_session-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
