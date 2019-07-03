---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1e10a4c3c846e59a6a05c5d7c57f838829209826
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458555"
---
# <a name="close-session"></a><span data-ttu-id="a7b81-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="a7b81-103">Close Session</span></span>

<span data-ttu-id="a7b81-104">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="a7b81-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a7b81-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7b81-105">Permissions</span></span>
<span data-ttu-id="a7b81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7b81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7b81-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7b81-108">Permission type</span></span>      | <span data-ttu-id="a7b81-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7b81-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7b81-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7b81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7b81-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7b81-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7b81-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7b81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7b81-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7b81-113">Not supported.</span></span>    |
|<span data-ttu-id="a7b81-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7b81-114">Application</span></span> | <span data-ttu-id="a7b81-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7b81-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7b81-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7b81-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="a7b81-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b81-117">Request headers</span></span>
| <span data-ttu-id="a7b81-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a7b81-118">Name</span></span>       | <span data-ttu-id="a7b81-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7b81-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7b81-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7b81-120">Authorization</span></span>  | <span data-ttu-id="a7b81-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7b81-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="a7b81-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a7b81-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a7b81-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a7b81-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="a7b81-126">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="a7b81-126">workbook-session-id</span></span> | <span data-ttu-id="a7b81-127">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="a7b81-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7b81-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b81-128">Request body</span></span>
<span data-ttu-id="a7b81-129">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7b81-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="a7b81-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7b81-130">Response</span></span>

<span data-ttu-id="a7b81-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7b81-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7b81-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7b81-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7b81-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b81-133">Request</span></span>
<span data-ttu-id="a7b81-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7b81-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7b81-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7b81-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7b81-136">C#</span><span class="sxs-lookup"><span data-stu-id="a7b81-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7b81-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7b81-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7b81-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a7b81-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a7b81-139">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="a7b81-139">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="a7b81-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7b81-140">Response</span></span>
<span data-ttu-id="a7b81-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7b81-141">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
