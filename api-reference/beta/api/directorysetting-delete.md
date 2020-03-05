---
title: Excluir uma configuração de diretório
description: Excluir uma configuração de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 16add1a6545740a068895c3af8c8a0afd3c66beb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434095"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="8c52b-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="8c52b-103">Delete a directory setting</span></span>

<span data-ttu-id="8c52b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c52b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c52b-105">Excluir uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="8c52b-105">Delete a directory setting.</span></span>

> <span data-ttu-id="8c52b-106">**Observação**: a versão do/beta desta API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="8c52b-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="8c52b-107">A versão/v1.0 dessa API foi renomeada para *excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="8c52b-107">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c52b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c52b-108">Permissions</span></span>
<span data-ttu-id="8c52b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c52b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c52b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c52b-111">Permission type</span></span>      | <span data-ttu-id="8c52b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c52b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c52b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c52b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c52b-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c52b-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c52b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c52b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c52b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c52b-116">Not supported.</span></span>    |
|<span data-ttu-id="8c52b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c52b-117">Application</span></span> | <span data-ttu-id="8c52b-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c52b-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c52b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c52b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8c52b-120">Excluir uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="8c52b-120">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8c52b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c52b-121">Request headers</span></span>
| <span data-ttu-id="8c52b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8c52b-122">Name</span></span>       | <span data-ttu-id="8c52b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c52b-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c52b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c52b-124">Authorization</span></span>  | <span data-ttu-id="8c52b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c52b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c52b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c52b-127">Request body</span></span>
<span data-ttu-id="8c52b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c52b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c52b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c52b-129">Response</span></span>

<span data-ttu-id="8c52b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c52b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c52b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c52b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c52b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c52b-133">Request</span></span>
<span data-ttu-id="8c52b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c52b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c52b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c52b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="8c52b-136">C#</span><span class="sxs-lookup"><span data-stu-id="8c52b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c52b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c52b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c52b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c52b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c52b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c52b-139">Response</span></span>
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
