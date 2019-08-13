---
title: Excluir uma configuração de diretório
description: Excluir uma configuração de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6821861196a923c73d44e3e5c5a70c0eda15d03e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319465"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="53ced-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="53ced-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53ced-104">Excluir uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="53ced-104">Delete a directory setting.</span></span>

> <span data-ttu-id="53ced-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="53ced-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="53ced-106">A versão/v1.0 dessa API foi renomeada para *excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="53ced-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="53ced-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="53ced-107">Permissions</span></span>
<span data-ttu-id="53ced-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53ced-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53ced-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53ced-110">Permission type</span></span>      | <span data-ttu-id="53ced-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53ced-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53ced-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53ced-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53ced-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53ced-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53ced-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53ced-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53ced-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53ced-115">Not supported.</span></span>    |
|<span data-ttu-id="53ced-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53ced-116">Application</span></span> | <span data-ttu-id="53ced-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53ced-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53ced-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53ced-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="53ced-119">Excluir uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="53ced-119">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="53ced-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53ced-120">Request headers</span></span>
| <span data-ttu-id="53ced-121">Nome</span><span class="sxs-lookup"><span data-stu-id="53ced-121">Name</span></span>       | <span data-ttu-id="53ced-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="53ced-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53ced-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53ced-123">Authorization</span></span>  | <span data-ttu-id="53ced-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53ced-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53ced-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53ced-126">Request body</span></span>
<span data-ttu-id="53ced-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53ced-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53ced-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="53ced-128">Response</span></span>

<span data-ttu-id="53ced-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53ced-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53ced-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53ced-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53ced-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53ced-132">Request</span></span>
<span data-ttu-id="53ced-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53ced-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="53ced-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="53ced-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53ced-135">C#</span><span class="sxs-lookup"><span data-stu-id="53ced-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53ced-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53ced-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53ced-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="53ced-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53ced-138">Java</span><span class="sxs-lookup"><span data-stu-id="53ced-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="53ced-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="53ced-139">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
