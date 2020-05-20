---
title: Excluir aplicativo
description: Excluir um objeto Application.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 67ab94c8d384141390195fd2818ced2d5d052dba
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289819"
---
# <a name="delete-application"></a><span data-ttu-id="da9d4-103">Excluir aplicativo</span><span class="sxs-lookup"><span data-stu-id="da9d4-103">Delete application</span></span>

<span data-ttu-id="da9d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da9d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da9d4-105">Excluir um objeto [Application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="da9d4-105">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="da9d4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="da9d4-106">Permissions</span></span>
<span data-ttu-id="da9d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da9d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da9d4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da9d4-109">Permission type</span></span>      | <span data-ttu-id="da9d4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da9d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da9d4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da9d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da9d4-112">Application. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="da9d4-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="da9d4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da9d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da9d4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da9d4-114">Not supported.</span></span>    |
|<span data-ttu-id="da9d4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da9d4-115">Application</span></span> | <span data-ttu-id="da9d4-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da9d4-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da9d4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da9d4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="da9d4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da9d4-118">Request headers</span></span>
| <span data-ttu-id="da9d4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="da9d4-119">Name</span></span>       | <span data-ttu-id="da9d4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="da9d4-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="da9d4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="da9d4-121">Authorization</span></span> | <span data-ttu-id="da9d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da9d4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da9d4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da9d4-124">Request body</span></span>
<span data-ttu-id="da9d4-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da9d4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da9d4-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="da9d4-126">Response</span></span>

<span data-ttu-id="da9d4-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da9d4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da9d4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da9d4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da9d4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da9d4-130">Request</span></span>
<span data-ttu-id="da9d4-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da9d4-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="da9d4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="da9d4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="da9d4-133">C#</span><span class="sxs-lookup"><span data-stu-id="da9d4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da9d4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da9d4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da9d4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da9d4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da9d4-136">Java</span><span class="sxs-lookup"><span data-stu-id="da9d4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="da9d4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="da9d4-137">Response</span></span>
<span data-ttu-id="da9d4-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da9d4-138">Here is an example of the response.</span></span> 
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
