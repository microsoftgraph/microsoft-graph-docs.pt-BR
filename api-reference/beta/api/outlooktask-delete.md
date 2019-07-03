---
title: Excluir outlookTask
description: Excluir a tarefa especificada do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 225db3d90fafecc7a33001b12f034f0419c37999
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450769"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="28467-103">Excluir outlookTask</span><span class="sxs-lookup"><span data-stu-id="28467-103">Delete outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28467-104">Excluir a tarefa especificada do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="28467-104">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="28467-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="28467-105">Permissions</span></span>

<span data-ttu-id="28467-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28467-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28467-108">Permission type</span></span>      | <span data-ttu-id="28467-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28467-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28467-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28467-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28467-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28467-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="28467-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28467-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28467-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28467-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="28467-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28467-114">Application</span></span> | <span data-ttu-id="28467-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28467-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28467-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28467-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28467-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28467-117">Request headers</span></span>

| <span data-ttu-id="28467-118">Nome</span><span class="sxs-lookup"><span data-stu-id="28467-118">Name</span></span>       | <span data-ttu-id="28467-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="28467-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28467-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="28467-120">Authorization</span></span>  | <span data-ttu-id="28467-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28467-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28467-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28467-123">Request body</span></span>

<span data-ttu-id="28467-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28467-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28467-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="28467-125">Response</span></span>

<span data-ttu-id="28467-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28467-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28467-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28467-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="28467-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28467-129">Request</span></span>

<span data-ttu-id="28467-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28467-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28467-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="28467-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28467-132">C#</span><span class="sxs-lookup"><span data-stu-id="28467-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28467-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="28467-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28467-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="28467-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28467-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="28467-135">Response</span></span>

<span data-ttu-id="28467-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28467-136">Here is an example of the response.</span></span>
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
