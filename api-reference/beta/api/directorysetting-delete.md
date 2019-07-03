---
title: Excluir uma configuração de diretório
description: Excluir uma configuração de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca08bfad3e6b18d81b5fc36223ae40b8bedcd4f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436827"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="d0398-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="d0398-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0398-104">Excluir uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="d0398-104">Delete a directory setting.</span></span>

> <span data-ttu-id="d0398-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="d0398-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d0398-106">A versão/v1.0 dessa API foi renomeada para *excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="d0398-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0398-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0398-107">Permissions</span></span>
<span data-ttu-id="d0398-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0398-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0398-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0398-110">Permission type</span></span>      | <span data-ttu-id="d0398-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0398-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0398-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0398-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0398-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0398-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0398-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0398-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0398-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0398-115">Not supported.</span></span>    |
|<span data-ttu-id="d0398-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0398-116">Application</span></span> | <span data-ttu-id="d0398-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0398-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0398-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0398-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d0398-119">Excluir uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="d0398-119">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d0398-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0398-120">Request headers</span></span>
| <span data-ttu-id="d0398-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d0398-121">Name</span></span>       | <span data-ttu-id="d0398-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0398-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d0398-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0398-123">Authorization</span></span>  | <span data-ttu-id="d0398-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0398-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0398-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0398-126">Request body</span></span>
<span data-ttu-id="d0398-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0398-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0398-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0398-128">Response</span></span>

<span data-ttu-id="d0398-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0398-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0398-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0398-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0398-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0398-132">Request</span></span>
<span data-ttu-id="d0398-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0398-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d0398-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0398-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d0398-135">C#</span><span class="sxs-lookup"><span data-stu-id="d0398-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0398-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0398-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d0398-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d0398-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0398-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0398-138">Response</span></span>
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
