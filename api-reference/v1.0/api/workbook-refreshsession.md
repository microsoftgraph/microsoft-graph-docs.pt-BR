---
title: Atualizar Sessão
description: 'Use esta API para atualizar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a79682ca4a1adbd7d3293307492b47098f6bda17
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365557"
---
# <a name="refresh-session"></a><span data-ttu-id="29aa2-103">Atualizar Sessão</span><span class="sxs-lookup"><span data-stu-id="29aa2-103">Refresh Session</span></span>

<span data-ttu-id="29aa2-104">Use esta API para atualizar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="29aa2-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="29aa2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="29aa2-105">Permissions</span></span>
<span data-ttu-id="29aa2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29aa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29aa2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29aa2-108">Permission type</span></span>      | <span data-ttu-id="29aa2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29aa2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29aa2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29aa2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29aa2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29aa2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29aa2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29aa2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29aa2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29aa2-113">Not supported.</span></span>    |
|<span data-ttu-id="29aa2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29aa2-114">Application</span></span> | <span data-ttu-id="29aa2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29aa2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29aa2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29aa2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="29aa2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29aa2-117">Request headers</span></span>
| <span data-ttu-id="29aa2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="29aa2-118">Name</span></span>       | <span data-ttu-id="29aa2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="29aa2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29aa2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="29aa2-120">Authorization</span></span>  | <span data-ttu-id="29aa2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29aa2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29aa2-123">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="29aa2-123">workbook-session-id</span></span> | <span data-ttu-id="29aa2-124">ID da sessão da pasta de trabalho a ser atualizada</span><span class="sxs-lookup"><span data-stu-id="29aa2-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="29aa2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29aa2-125">Request body</span></span>
<span data-ttu-id="29aa2-126">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29aa2-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="29aa2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="29aa2-127">Response</span></span>

<span data-ttu-id="29aa2-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="29aa2-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="29aa2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29aa2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29aa2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29aa2-130">Request</span></span>
<span data-ttu-id="29aa2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29aa2-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="29aa2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="29aa2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29aa2-133">C#</span><span class="sxs-lookup"><span data-stu-id="29aa2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29aa2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29aa2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29aa2-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="29aa2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="29aa2-136">Java</span><span class="sxs-lookup"><span data-stu-id="29aa2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/refresh-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="29aa2-137">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="29aa2-137">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="29aa2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="29aa2-138">Response</span></span>
<span data-ttu-id="29aa2-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29aa2-139">Here is an example of the response.</span></span> 

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
    "Warning: refresh_excel_session//api-reference/v1.0/api/workbook-refreshsession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
