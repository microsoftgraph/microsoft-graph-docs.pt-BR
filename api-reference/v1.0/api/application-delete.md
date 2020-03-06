---
title: Excluir aplicativo
description: Excluir um objeto Application.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 942791a5c35d8a6202abab0cf7ab13ec7d9943df
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518921"
---
# <a name="delete-application"></a><span data-ttu-id="ac8a0-103">Excluir aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac8a0-103">Delete application</span></span>

<span data-ttu-id="ac8a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac8a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac8a0-105">Excluir um objeto [Application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="ac8a0-105">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac8a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac8a0-106">Permissions</span></span>
<span data-ttu-id="ac8a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac8a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac8a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac8a0-109">Permission type</span></span>      | <span data-ttu-id="ac8a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac8a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac8a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac8a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ac8a0-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac8a0-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac8a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac8a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac8a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac8a0-114">Not supported.</span></span>    |
|<span data-ttu-id="ac8a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac8a0-115">Application</span></span> | <span data-ttu-id="ac8a0-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac8a0-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac8a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac8a0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ac8a0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac8a0-118">Request headers</span></span>
| <span data-ttu-id="ac8a0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ac8a0-119">Name</span></span>       | <span data-ttu-id="ac8a0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac8a0-120">Type</span></span> | <span data-ttu-id="ac8a0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac8a0-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac8a0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac8a0-122">Authorization</span></span>  | <span data-ttu-id="ac8a0-123">string</span><span class="sxs-lookup"><span data-stu-id="ac8a0-123">string</span></span>  | <span data-ttu-id="ac8a0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac8a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac8a0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac8a0-126">Request body</span></span>
<span data-ttu-id="ac8a0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac8a0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac8a0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac8a0-128">Response</span></span>

<span data-ttu-id="ac8a0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac8a0-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac8a0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac8a0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac8a0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac8a0-132">Request</span></span>
<span data-ttu-id="ac8a0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac8a0-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ac8a0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac8a0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="ac8a0-135">C#</span><span class="sxs-lookup"><span data-stu-id="ac8a0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac8a0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac8a0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac8a0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac8a0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac8a0-138">Java</span><span class="sxs-lookup"><span data-stu-id="ac8a0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac8a0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac8a0-139">Response</span></span>
<span data-ttu-id="ac8a0-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac8a0-140">Here is an example of the response.</span></span> 
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
