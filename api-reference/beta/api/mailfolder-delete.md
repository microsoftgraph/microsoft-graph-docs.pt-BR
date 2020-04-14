---
title: Excluir mailFolder
description: Exclua o mailFolder ou o mailSearchFolder especificado.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b09329fd2e39ecd2e59e53b04aebfaaed5c13651
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457149"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="00eed-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="00eed-103">Delete mailFolder</span></span>

<span data-ttu-id="00eed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00eed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00eed-105">Exclua o [mailFolder](../resources/mailfolder.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="00eed-105">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="00eed-106">A pasta pode ser uma [mailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="00eed-106">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="00eed-107">Você pode especificar uma pasta de email por sua ID de pasta ou por seu [nome de pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="00eed-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span>

><span data-ttu-id="00eed-108">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo nome `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="00eed-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="00eed-109">Veja [retenção de item excluído](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="00eed-109">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="00eed-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="00eed-110">Permissions</span></span>
<span data-ttu-id="00eed-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00eed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00eed-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00eed-113">Permission type</span></span>      | <span data-ttu-id="00eed-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00eed-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00eed-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00eed-115">Delegated (work or school account)</span></span> | <span data-ttu-id="00eed-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00eed-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="00eed-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00eed-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00eed-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00eed-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="00eed-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00eed-119">Application</span></span> | <span data-ttu-id="00eed-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00eed-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="00eed-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00eed-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="00eed-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00eed-122">Request headers</span></span>
| <span data-ttu-id="00eed-123">Nome</span><span class="sxs-lookup"><span data-stu-id="00eed-123">Name</span></span>       | <span data-ttu-id="00eed-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="00eed-124">Type</span></span> | <span data-ttu-id="00eed-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="00eed-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="00eed-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="00eed-126">Authorization</span></span>  | <span data-ttu-id="00eed-127">string</span><span class="sxs-lookup"><span data-stu-id="00eed-127">string</span></span>  | <span data-ttu-id="00eed-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00eed-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00eed-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00eed-130">Request body</span></span>
<span data-ttu-id="00eed-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00eed-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00eed-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="00eed-132">Response</span></span>
<span data-ttu-id="00eed-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00eed-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00eed-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00eed-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="00eed-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00eed-136">Request</span></span>
<span data-ttu-id="00eed-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="00eed-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00eed-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="00eed-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```
# <a name="c"></a>[<span data-ttu-id="00eed-139">C#</span><span class="sxs-lookup"><span data-stu-id="00eed-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00eed-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00eed-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00eed-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00eed-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="00eed-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="00eed-142">Response</span></span>
<span data-ttu-id="00eed-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="00eed-143">The following is an example of the response.</span></span>
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
