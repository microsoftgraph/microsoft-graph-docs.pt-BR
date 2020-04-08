---
title: Excluir uma configuração de diretório
description: Excluir uma configuração de diretório.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 27eb77aebf0dac6eac352f370088d8729952ff96
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180841"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="304c7-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="304c7-103">Delete a directory setting</span></span>

<span data-ttu-id="304c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="304c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="304c7-105">Excluir uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="304c7-105">Delete a directory setting.</span></span>

> <span data-ttu-id="304c7-106">**Observação**: a versão do/beta desta API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="304c7-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="304c7-107">A versão/v1.0 dessa API foi renomeada para *excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="304c7-107">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="304c7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="304c7-108">Permissions</span></span>
<span data-ttu-id="304c7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="304c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="304c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="304c7-111">Permission type</span></span>      | <span data-ttu-id="304c7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="304c7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="304c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="304c7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="304c7-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="304c7-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="304c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="304c7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="304c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="304c7-116">Not supported.</span></span>    |
|<span data-ttu-id="304c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="304c7-117">Application</span></span> | <span data-ttu-id="304c7-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304c7-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="304c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="304c7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="304c7-120">Excluir uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="304c7-120">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="304c7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="304c7-121">Request headers</span></span>
| <span data-ttu-id="304c7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="304c7-122">Name</span></span>       | <span data-ttu-id="304c7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="304c7-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="304c7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="304c7-124">Authorization</span></span>  | <span data-ttu-id="304c7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="304c7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="304c7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="304c7-127">Request body</span></span>
<span data-ttu-id="304c7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="304c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="304c7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="304c7-129">Response</span></span>

<span data-ttu-id="304c7-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="304c7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="304c7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="304c7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="304c7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="304c7-133">Request</span></span>
<span data-ttu-id="304c7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="304c7-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="304c7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="304c7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="304c7-136">C#</span><span class="sxs-lookup"><span data-stu-id="304c7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="304c7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="304c7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="304c7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="304c7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="304c7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="304c7-139">Response</span></span>
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
