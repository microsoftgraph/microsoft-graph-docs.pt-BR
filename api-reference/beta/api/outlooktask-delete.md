---
title: Excluir outlookTask
description: Excluir a tarefa especificada do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 76aab2a7598ad380c5b1841428a5b0740c07d662
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988703"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="874e1-103">Excluir outlookTask</span><span class="sxs-lookup"><span data-stu-id="874e1-103">Delete outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="874e1-104">Excluir a tarefa especificada do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="874e1-104">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="874e1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="874e1-105">Permissions</span></span>

<span data-ttu-id="874e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="874e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="874e1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="874e1-108">Permission type</span></span>      | <span data-ttu-id="874e1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="874e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="874e1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="874e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="874e1-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="874e1-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="874e1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="874e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="874e1-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="874e1-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="874e1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="874e1-114">Application</span></span> | <span data-ttu-id="874e1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="874e1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="874e1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="874e1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="874e1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="874e1-117">Request headers</span></span>

| <span data-ttu-id="874e1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="874e1-118">Name</span></span>       | <span data-ttu-id="874e1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="874e1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="874e1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="874e1-120">Authorization</span></span>  | <span data-ttu-id="874e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="874e1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="874e1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="874e1-123">Request body</span></span>

<span data-ttu-id="874e1-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="874e1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="874e1-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="874e1-125">Response</span></span>

<span data-ttu-id="874e1-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="874e1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="874e1-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="874e1-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="874e1-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874e1-129">Request</span></span>

<span data-ttu-id="874e1-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="874e1-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="874e1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="874e1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="874e1-132">C#</span><span class="sxs-lookup"><span data-stu-id="874e1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="874e1-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="874e1-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="874e1-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="874e1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="874e1-135">Java</span><span class="sxs-lookup"><span data-stu-id="874e1-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="874e1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="874e1-136">Response</span></span>

<span data-ttu-id="874e1-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="874e1-137">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
