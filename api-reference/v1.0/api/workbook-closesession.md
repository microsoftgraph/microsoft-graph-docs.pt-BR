---
title: Fechar sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b1dd8a20fdfda223f4a757d6c9df661fb66b7c85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970905"
---
# <a name="close-session"></a><span data-ttu-id="abc51-103">Fechar sessão</span><span class="sxs-lookup"><span data-stu-id="abc51-103">Close Session</span></span>

<span data-ttu-id="abc51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abc51-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="abc51-105">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="abc51-105">Use this API to close an existing workbook session.</span></span>

## <a name="permissions"></a><span data-ttu-id="abc51-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="abc51-106">Permissions</span></span>
<span data-ttu-id="abc51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abc51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abc51-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abc51-109">Permission type</span></span>      | <span data-ttu-id="abc51-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abc51-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abc51-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abc51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="abc51-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abc51-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="abc51-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abc51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abc51-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abc51-114">Not supported.</span></span>    |
|<span data-ttu-id="abc51-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abc51-115">Application</span></span> | <span data-ttu-id="abc51-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abc51-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abc51-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abc51-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="abc51-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abc51-118">Request headers</span></span>
| <span data-ttu-id="abc51-119">Nome</span><span class="sxs-lookup"><span data-stu-id="abc51-119">Name</span></span>                | <span data-ttu-id="abc51-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="abc51-120">Description</span></span>                      |
|:--------------------|:---------------------------------|
| <span data-ttu-id="abc51-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="abc51-121">Authorization</span></span>       | <span data-ttu-id="abc51-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abc51-p102">Bearer {token}. Required.</span></span>        |
| <span data-ttu-id="abc51-124">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="abc51-124">workbook-session-id</span></span> | <span data-ttu-id="abc51-125">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="abc51-125">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="abc51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abc51-126">Request body</span></span>
<span data-ttu-id="abc51-127">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="abc51-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="abc51-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="abc51-128">Response</span></span>

<span data-ttu-id="abc51-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="abc51-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="abc51-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abc51-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abc51-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abc51-131">Request</span></span>
<span data-ttu-id="abc51-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abc51-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="abc51-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="abc51-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="abc51-134">C#</span><span class="sxs-lookup"><span data-stu-id="abc51-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/close-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abc51-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abc51-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/close-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abc51-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abc51-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/close-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abc51-137">Java</span><span class="sxs-lookup"><span data-stu-id="abc51-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/close-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="abc51-138">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="abc51-138">Note that workbook-session-id header is required.</span></span>


##### <a name="response"></a><span data-ttu-id="abc51-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="abc51-139">Response</span></span>
<span data-ttu-id="abc51-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abc51-140">Here is an example of the response.</span></span>

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

