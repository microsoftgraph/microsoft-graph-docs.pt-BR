---
title: Excluir uma configuração de diretório
description: Excluir uma configuração de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4036e6bb6ade07c8c2998aff94c099d27d2dcad0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417210"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="97211-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="97211-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97211-104">Excluir uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="97211-104">Delete a directory setting.</span></span>

> <span data-ttu-id="97211-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="97211-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="97211-106">A versão/v1.0 dessa API foi renomeada para *excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="97211-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="97211-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="97211-107">Permissions</span></span>
<span data-ttu-id="97211-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97211-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97211-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97211-110">Permission type</span></span>      | <span data-ttu-id="97211-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97211-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97211-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97211-112">Delegated (work or school account)</span></span> | <span data-ttu-id="97211-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97211-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97211-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97211-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97211-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97211-115">Not supported.</span></span>    |
|<span data-ttu-id="97211-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97211-116">Application</span></span> | <span data-ttu-id="97211-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97211-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97211-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97211-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="97211-119">Excluir uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="97211-119">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="97211-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97211-120">Request headers</span></span>
| <span data-ttu-id="97211-121">Nome</span><span class="sxs-lookup"><span data-stu-id="97211-121">Name</span></span>       | <span data-ttu-id="97211-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="97211-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97211-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97211-123">Authorization</span></span>  | <span data-ttu-id="97211-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97211-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97211-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97211-126">Request body</span></span>
<span data-ttu-id="97211-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97211-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97211-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="97211-128">Response</span></span>

<span data-ttu-id="97211-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97211-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97211-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97211-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97211-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97211-132">Request</span></span>
<span data-ttu-id="97211-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97211-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="97211-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="97211-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97211-135">C#</span><span class="sxs-lookup"><span data-stu-id="97211-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97211-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97211-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97211-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="97211-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="97211-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="97211-138">Response</span></span>
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
