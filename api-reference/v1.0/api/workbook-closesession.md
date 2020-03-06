---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ee16d09d61df2f805d7af50748935a588e578c1b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508881"
---
# <a name="close-session"></a><span data-ttu-id="a9500-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="a9500-103">Close Session</span></span>

<span data-ttu-id="a9500-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9500-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9500-105">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="a9500-105">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a9500-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9500-106">Permissions</span></span>
<span data-ttu-id="a9500-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9500-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9500-109">Permission type</span></span>      | <span data-ttu-id="a9500-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9500-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9500-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9500-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9500-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9500-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a9500-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9500-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9500-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9500-114">Not supported.</span></span>    |
|<span data-ttu-id="a9500-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9500-115">Application</span></span> | <span data-ttu-id="a9500-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9500-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9500-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9500-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="a9500-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9500-118">Request headers</span></span>
| <span data-ttu-id="a9500-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a9500-119">Name</span></span>       | <span data-ttu-id="a9500-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9500-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a9500-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9500-121">Authorization</span></span>  | <span data-ttu-id="a9500-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9500-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="a9500-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a9500-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a9500-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a9500-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="a9500-127">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="a9500-127">workbook-session-id</span></span> | <span data-ttu-id="a9500-128">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="a9500-128">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9500-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9500-129">Request body</span></span>
<span data-ttu-id="a9500-130">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9500-130">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="a9500-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9500-131">Response</span></span>

<span data-ttu-id="a9500-132">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a9500-132">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9500-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9500-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9500-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9500-134">Request</span></span>
<span data-ttu-id="a9500-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9500-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9500-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9500-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a9500-137">C#</span><span class="sxs-lookup"><span data-stu-id="a9500-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9500-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9500-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9500-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9500-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9500-140">Java</span><span class="sxs-lookup"><span data-stu-id="a9500-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/close-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a9500-141">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="a9500-141">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="a9500-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9500-142">Response</span></span>
<span data-ttu-id="a9500-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9500-143">Here is an example of the response.</span></span> 

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
