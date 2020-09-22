---
title: Remover membro
description: Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: da44682e05582581373ac456c12db7df7a731270
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094845"
---
# <a name="remove-member"></a><span data-ttu-id="0d23e-103">Remover membro</span><span class="sxs-lookup"><span data-stu-id="0d23e-103">Remove member</span></span>

<span data-ttu-id="0d23e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d23e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d23e-105">Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.</span><span class="sxs-lookup"><span data-stu-id="0d23e-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d23e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d23e-106">Permissions</span></span>
<span data-ttu-id="0d23e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d23e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d23e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d23e-109">Permission type</span></span>      | <span data-ttu-id="0d23e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d23e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d23e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d23e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d23e-112">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d23e-112">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0d23e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d23e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d23e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d23e-114">Not supported.</span></span> |
|<span data-ttu-id="0d23e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d23e-115">Application</span></span> | <span data-ttu-id="0d23e-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d23e-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d23e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d23e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0d23e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d23e-118">Request headers</span></span>
| <span data-ttu-id="0d23e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0d23e-119">Name</span></span>       | <span data-ttu-id="0d23e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d23e-120">Type</span></span> | <span data-ttu-id="0d23e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d23e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d23e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d23e-122">Authorization</span></span>  | <span data-ttu-id="0d23e-123">string</span><span class="sxs-lookup"><span data-stu-id="0d23e-123">string</span></span>  | <span data-ttu-id="0d23e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d23e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d23e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d23e-126">Request body</span></span>
<span data-ttu-id="0d23e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d23e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d23e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d23e-128">Response</span></span>
<span data-ttu-id="0d23e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d23e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d23e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d23e-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0d23e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d23e-132">Request</span></span>
<span data-ttu-id="0d23e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d23e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d23e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d23e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="0d23e-135">C#</span><span class="sxs-lookup"><span data-stu-id="0d23e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d23e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d23e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d23e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d23e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d23e-138">Java</span><span class="sxs-lookup"><span data-stu-id="0d23e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0d23e-139">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="0d23e-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="0d23e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d23e-140">Response</span></span>
<span data-ttu-id="0d23e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d23e-141">The following is an example of the response.</span></span>
><span data-ttu-id="0d23e-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d23e-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0d23e-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d23e-143">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

