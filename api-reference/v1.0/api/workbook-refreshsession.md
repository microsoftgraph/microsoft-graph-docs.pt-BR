---
title: Atualizar sessão
description: 'Use esta API para atualizar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 05ec3fc978efdeec23ba49ce2ba310278b3be28d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970821"
---
# <a name="refresh-session"></a><span data-ttu-id="93f84-103">Atualizar sessão</span><span class="sxs-lookup"><span data-stu-id="93f84-103">Refresh Session</span></span>

<span data-ttu-id="93f84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f84-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93f84-105">Use esta API para atualizar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="93f84-105">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="93f84-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93f84-106">Permissions</span></span>
<span data-ttu-id="93f84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93f84-109">Permission type</span></span>      | <span data-ttu-id="93f84-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93f84-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93f84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93f84-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93f84-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93f84-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="93f84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93f84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93f84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93f84-114">Not supported.</span></span>    |
|<span data-ttu-id="93f84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93f84-115">Application</span></span> | <span data-ttu-id="93f84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93f84-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93f84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93f84-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="93f84-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93f84-118">Request headers</span></span>
| <span data-ttu-id="93f84-119">Nome</span><span class="sxs-lookup"><span data-stu-id="93f84-119">Name</span></span>       | <span data-ttu-id="93f84-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="93f84-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="93f84-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="93f84-121">Authorization</span></span>  | <span data-ttu-id="93f84-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93f84-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93f84-124">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="93f84-124">workbook-session-id</span></span> | <span data-ttu-id="93f84-125">ID da sessão da pasta de trabalho a ser atualizada</span><span class="sxs-lookup"><span data-stu-id="93f84-125">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="93f84-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93f84-126">Request body</span></span>
<span data-ttu-id="93f84-127">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93f84-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="93f84-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f84-128">Response</span></span>

<span data-ttu-id="93f84-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="93f84-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="93f84-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93f84-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93f84-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93f84-131">Request</span></span>
<span data-ttu-id="93f84-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93f84-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93f84-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="93f84-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="93f84-134">C#</span><span class="sxs-lookup"><span data-stu-id="93f84-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93f84-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93f84-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93f84-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93f84-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93f84-137">Java</span><span class="sxs-lookup"><span data-stu-id="93f84-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/refresh-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="93f84-138">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="93f84-138">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="93f84-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f84-139">Response</span></span>
<span data-ttu-id="93f84-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93f84-140">Here is an example of the response.</span></span> 

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

