---
title: Excluir uma configuração de diretório
description: Excluir uma configuração de diretório.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0d1459e7ace8a2de6bae4fc696ac308cffca6392
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436691"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="a21ca-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="a21ca-103">Delete a directory setting</span></span>

<span data-ttu-id="a21ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a21ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a21ca-105">Excluir uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="a21ca-105">Delete a directory setting.</span></span>

> <span data-ttu-id="a21ca-106">**Observação**: a versão /beta dessa API só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="a21ca-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="a21ca-107">A versão /v1.0 desta API foi renomeada para *Excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="a21ca-107">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="a21ca-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a21ca-108">Permissions</span></span>
<span data-ttu-id="a21ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a21ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a21ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a21ca-111">Permission type</span></span>      | <span data-ttu-id="a21ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a21ca-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a21ca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a21ca-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a21ca-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a21ca-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a21ca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a21ca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a21ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a21ca-116">Not supported.</span></span>    |
|<span data-ttu-id="a21ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a21ca-117">Application</span></span> | <span data-ttu-id="a21ca-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a21ca-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a21ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a21ca-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a21ca-120">Excluir uma configuração específica de grupo ou de locatário</span><span class="sxs-lookup"><span data-stu-id="a21ca-120">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a21ca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a21ca-121">Request headers</span></span>
| <span data-ttu-id="a21ca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a21ca-122">Name</span></span>       | <span data-ttu-id="a21ca-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a21ca-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a21ca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a21ca-124">Authorization</span></span>  | <span data-ttu-id="a21ca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a21ca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a21ca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a21ca-127">Request body</span></span>
<span data-ttu-id="a21ca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a21ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a21ca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a21ca-129">Response</span></span>

<span data-ttu-id="a21ca-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a21ca-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a21ca-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a21ca-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a21ca-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a21ca-133">Request</span></span>
<span data-ttu-id="a21ca-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a21ca-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a21ca-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a21ca-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="a21ca-136">C#</span><span class="sxs-lookup"><span data-stu-id="a21ca-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a21ca-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a21ca-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a21ca-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a21ca-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a21ca-139">Java</span><span class="sxs-lookup"><span data-stu-id="a21ca-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a21ca-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a21ca-140">Response</span></span>
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


