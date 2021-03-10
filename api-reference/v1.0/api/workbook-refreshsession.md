---
title: Atualizar Sessão
description: 'Use essa API para atualizar uma sessão de workbook existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5e4aaad295abc4ce83b8669f3d4053edafb1ad5d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575837"
---
# <a name="refresh-session"></a><span data-ttu-id="45c22-103">Atualizar Sessão</span><span class="sxs-lookup"><span data-stu-id="45c22-103">Refresh Session</span></span>

<span data-ttu-id="45c22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45c22-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45c22-105">Use essa API para atualizar uma sessão de workbook existente.</span><span class="sxs-lookup"><span data-stu-id="45c22-105">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="45c22-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45c22-106">Permissions</span></span>
<span data-ttu-id="45c22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45c22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c22-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45c22-109">Permission type</span></span>      | <span data-ttu-id="45c22-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45c22-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45c22-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45c22-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45c22-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45c22-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="45c22-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45c22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45c22-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45c22-114">Not supported.</span></span>    |
|<span data-ttu-id="45c22-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45c22-115">Application</span></span> | <span data-ttu-id="45c22-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45c22-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45c22-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45c22-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/refreshSession
POST /me/drive/root:/{item-path}:/workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="45c22-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45c22-118">Request headers</span></span>
| <span data-ttu-id="45c22-119">Nome</span><span class="sxs-lookup"><span data-stu-id="45c22-119">Name</span></span>       | <span data-ttu-id="45c22-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="45c22-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45c22-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="45c22-121">Authorization</span></span>  | <span data-ttu-id="45c22-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45c22-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45c22-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="45c22-124">workbook-session-id</span></span> | <span data-ttu-id="45c22-125">ID da sessão de workbook a ser atualizada</span><span class="sxs-lookup"><span data-stu-id="45c22-125">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="45c22-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45c22-126">Request body</span></span>
<span data-ttu-id="45c22-127">Essa API não exige nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45c22-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="45c22-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c22-128">Response</span></span>

<span data-ttu-id="45c22-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45c22-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45c22-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45c22-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45c22-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45c22-131">Request</span></span>
<span data-ttu-id="45c22-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45c22-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45c22-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="45c22-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="45c22-134">C#</span><span class="sxs-lookup"><span data-stu-id="45c22-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45c22-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45c22-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45c22-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45c22-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45c22-137">Java</span><span class="sxs-lookup"><span data-stu-id="45c22-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/refresh-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="45c22-138">Observe que o header workbook-session-id é necessário.</span><span class="sxs-lookup"><span data-stu-id="45c22-138">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="45c22-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c22-139">Response</span></span>
<span data-ttu-id="45c22-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45c22-140">Here is an example of the response.</span></span> 

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
  ]
}-->

