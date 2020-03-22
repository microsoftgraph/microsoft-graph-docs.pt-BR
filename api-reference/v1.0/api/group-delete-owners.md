---
title: Remover proprietário
description: Use esta API para remover um proprietário de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 87880e417af00695b3644fac87d47db5d91f8047
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892636"
---
# <a name="remove-owner"></a><span data-ttu-id="a64af-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="a64af-103">Remove owner</span></span>

<span data-ttu-id="a64af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a64af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a64af-105">Use esta API para remover um proprietário de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação owners.</span><span class="sxs-lookup"><span data-stu-id="a64af-105">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a64af-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a64af-106">Permissions</span></span>
<span data-ttu-id="a64af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a64af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a64af-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a64af-109">Permission type</span></span>      | <span data-ttu-id="a64af-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a64af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a64af-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a64af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a64af-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a64af-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a64af-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a64af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a64af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a64af-114">Not supported.</span></span>    |
|<span data-ttu-id="a64af-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a64af-115">Application</span></span> | <span data-ttu-id="a64af-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a64af-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a64af-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a64af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a64af-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a64af-118">Request headers</span></span>
| <span data-ttu-id="a64af-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a64af-119">Name</span></span>       | <span data-ttu-id="a64af-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a64af-120">Type</span></span> | <span data-ttu-id="a64af-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a64af-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a64af-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a64af-122">Authorization</span></span>  | <span data-ttu-id="a64af-123">string</span><span class="sxs-lookup"><span data-stu-id="a64af-123">string</span></span>  | <span data-ttu-id="a64af-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a64af-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a64af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a64af-126">Request body</span></span>
<span data-ttu-id="a64af-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a64af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a64af-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a64af-128">Response</span></span>
<span data-ttu-id="a64af-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a64af-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a64af-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a64af-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a64af-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a64af-132">Request</span></span>
<span data-ttu-id="a64af-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a64af-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a64af-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a64af-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="a64af-135">C#</span><span class="sxs-lookup"><span data-stu-id="a64af-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a64af-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a64af-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a64af-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a64af-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a64af-138">Java</span><span class="sxs-lookup"><span data-stu-id="a64af-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a64af-139">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="a64af-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="a64af-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a64af-140">Response</span></span>
<span data-ttu-id="a64af-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a64af-141">The following is an example of the response.</span></span>
><span data-ttu-id="a64af-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a64af-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a64af-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a64af-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
