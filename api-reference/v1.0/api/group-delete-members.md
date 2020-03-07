---
title: Remover membro
description: Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 54066ba22f34481bd213806909dc0f826d6860d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517191"
---
# <a name="remove-member"></a><span data-ttu-id="24edf-103">Remover membro</span><span class="sxs-lookup"><span data-stu-id="24edf-103">Remove member</span></span>

<span data-ttu-id="24edf-104">Namespace: microsoft.graph Use essa API para remover um membro de um grupo por meio da propriedade de navegação **membros**.</span><span class="sxs-lookup"><span data-stu-id="24edf-104">Namespace: microsoft.graph Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="24edf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="24edf-105">Permissions</span></span>
<span data-ttu-id="24edf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24edf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24edf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24edf-108">Permission type</span></span>      | <span data-ttu-id="24edf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24edf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24edf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24edf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24edf-111">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="24edf-111">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="24edf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24edf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24edf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24edf-113">Not supported.</span></span> |
|<span data-ttu-id="24edf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24edf-114">Application</span></span> | <span data-ttu-id="24edf-115">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24edf-115">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24edf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24edf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="24edf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24edf-117">Request headers</span></span>
| <span data-ttu-id="24edf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="24edf-118">Name</span></span>       | <span data-ttu-id="24edf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="24edf-119">Type</span></span> | <span data-ttu-id="24edf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="24edf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24edf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="24edf-121">Authorization</span></span>  | <span data-ttu-id="24edf-122">string</span><span class="sxs-lookup"><span data-stu-id="24edf-122">string</span></span>  | <span data-ttu-id="24edf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24edf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24edf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24edf-125">Request body</span></span>
<span data-ttu-id="24edf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24edf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24edf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="24edf-127">Response</span></span>
<span data-ttu-id="24edf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24edf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24edf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24edf-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="24edf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24edf-131">Request</span></span>
<span data-ttu-id="24edf-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="24edf-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="24edf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="24edf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="24edf-134">C#</span><span class="sxs-lookup"><span data-stu-id="24edf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24edf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24edf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24edf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24edf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24edf-137">Java</span><span class="sxs-lookup"><span data-stu-id="24edf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="24edf-138">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="24edf-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="24edf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="24edf-139">Response</span></span>
<span data-ttu-id="24edf-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24edf-140">The following is an example of the response.</span></span>
><span data-ttu-id="24edf-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24edf-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="24edf-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24edf-142">All the properties will be returned from an actual call.</span></span>
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
