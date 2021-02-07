---
title: Excluir aplicativo
description: Exclua um objeto application.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: da60fd5c6a3a97a3924fc45448c00f9665748752
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131779"
---
# <a name="delete-application"></a><span data-ttu-id="999f7-103">Excluir aplicativo</span><span class="sxs-lookup"><span data-stu-id="999f7-103">Delete application</span></span>

<span data-ttu-id="999f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="999f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="999f7-105">Exclua [um objeto application.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="999f7-105">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="999f7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="999f7-106">Permissions</span></span>
<span data-ttu-id="999f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="999f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="999f7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="999f7-109">Permission type</span></span>      | <span data-ttu-id="999f7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="999f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="999f7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="999f7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="999f7-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="999f7-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="999f7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="999f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="999f7-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="999f7-114">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="999f7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="999f7-115">Application</span></span> | <span data-ttu-id="999f7-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="999f7-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="999f7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="999f7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="999f7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="999f7-118">Request headers</span></span>
| <span data-ttu-id="999f7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="999f7-119">Name</span></span>       | <span data-ttu-id="999f7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="999f7-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="999f7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="999f7-121">Authorization</span></span> | <span data-ttu-id="999f7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="999f7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="999f7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="999f7-124">Request body</span></span>
<span data-ttu-id="999f7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="999f7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="999f7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="999f7-126">Response</span></span>

<span data-ttu-id="999f7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="999f7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="999f7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="999f7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="999f7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="999f7-130">Request</span></span>
<span data-ttu-id="999f7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="999f7-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="999f7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="999f7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="999f7-133">C#</span><span class="sxs-lookup"><span data-stu-id="999f7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="999f7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="999f7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="999f7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="999f7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="999f7-136">Java</span><span class="sxs-lookup"><span data-stu-id="999f7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="999f7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="999f7-137">Response</span></span>
<span data-ttu-id="999f7-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="999f7-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

