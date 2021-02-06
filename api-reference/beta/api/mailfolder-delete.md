---
title: Excluir mailFolder
description: Exclua a mailFolder ou mailSearchFolder especificada.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2574d3e220e61fb7fa7a61c8c23240348a1594c7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136756"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="2dd3e-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="2dd3e-103">Delete mailFolder</span></span>

<span data-ttu-id="2dd3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dd3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dd3e-105">Exclua a [mailFolder especificada.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="2dd3e-105">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="2dd3e-106">A pasta pode ser [uma mailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="2dd3e-106">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="2dd3e-107">Você pode especificar uma pasta de email por sua ID de pasta ou por seu nome [de](../resources/mailfolder.md)pasta conhecido, se houver uma.</span><span class="sxs-lookup"><span data-stu-id="2dd3e-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span>

><span data-ttu-id="2dd3e-108">**Observação** Talvez você não consiga excluir itens na pasta de exclusões de itens recuperáveis (representado pelo nome de pasta `recoverableitemsdeletions` conhecido).</span><span class="sxs-lookup"><span data-stu-id="2dd3e-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="2dd3e-109">Consulte [Retenção de itens excluídos](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e Limpar itens [excluídos](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="2dd3e-109">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="2dd3e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2dd3e-110">Permissions</span></span>
<span data-ttu-id="2dd3e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dd3e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dd3e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2dd3e-113">Permission type</span></span>      | <span data-ttu-id="2dd3e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2dd3e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dd3e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2dd3e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2dd3e-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dd3e-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2dd3e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2dd3e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dd3e-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dd3e-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2dd3e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2dd3e-119">Application</span></span> | <span data-ttu-id="2dd3e-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dd3e-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dd3e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2dd3e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2dd3e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2dd3e-122">Request headers</span></span>
| <span data-ttu-id="2dd3e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="2dd3e-123">Name</span></span>       | <span data-ttu-id="2dd3e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dd3e-124">Type</span></span> | <span data-ttu-id="2dd3e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dd3e-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2dd3e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2dd3e-126">Authorization</span></span>  | <span data-ttu-id="2dd3e-127">string</span><span class="sxs-lookup"><span data-stu-id="2dd3e-127">string</span></span>  | <span data-ttu-id="2dd3e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2dd3e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2dd3e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2dd3e-130">Request body</span></span>
<span data-ttu-id="2dd3e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2dd3e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2dd3e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dd3e-132">Response</span></span>
<span data-ttu-id="2dd3e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2dd3e-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dd3e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2dd3e-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2dd3e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2dd3e-136">Request</span></span>
<span data-ttu-id="2dd3e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2dd3e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2dd3e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2dd3e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```
# <a name="c"></a>[<span data-ttu-id="2dd3e-139">C#</span><span class="sxs-lookup"><span data-stu-id="2dd3e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2dd3e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dd3e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2dd3e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2dd3e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2dd3e-142">Java</span><span class="sxs-lookup"><span data-stu-id="2dd3e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2dd3e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dd3e-143">Response</span></span>
<span data-ttu-id="2dd3e-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2dd3e-144">The following is an example of the response.</span></span>
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


