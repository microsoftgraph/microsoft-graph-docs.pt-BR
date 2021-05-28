---
title: Remover proprietário
description: Use essa API para remover um proprietário de um grupo de Microsoft 365, um grupo de segurança ou um grupo de segurança habilitado para email por meio da propriedade de navegação de proprietários.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 34a7dcd31642f56d34aacc05082ef57c801e5e6a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680980"
---
# <a name="remove-owner"></a><span data-ttu-id="b15d3-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="b15d3-103">Remove owner</span></span>

<span data-ttu-id="b15d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b15d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b15d3-105">Use essa API para remover um proprietário de um grupo de Microsoft 365, um grupo de segurança ou um grupo de segurança habilitado para email por meio da propriedade de navegação de proprietários.</span><span class="sxs-lookup"><span data-stu-id="b15d3-105">Use this API to remove an owner from a Microsoft 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span> <span data-ttu-id="b15d3-106">Depois que os proprietários são atribuídos a um grupo, o último proprietário do grupo não pode ser removido.</span><span class="sxs-lookup"><span data-stu-id="b15d3-106">Once owners are assigned to a group, the last owner of the group cannot be removed.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b15d3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b15d3-107">Permissions</span></span>
<span data-ttu-id="b15d3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b15d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b15d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b15d3-110">Permission type</span></span>      | <span data-ttu-id="b15d3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b15d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b15d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b15d3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b15d3-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b15d3-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b15d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b15d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b15d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b15d3-115">Not supported.</span></span>    |
|<span data-ttu-id="b15d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b15d3-116">Application</span></span> | <span data-ttu-id="b15d3-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b15d3-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b15d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b15d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b15d3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b15d3-119">Request headers</span></span>
| <span data-ttu-id="b15d3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b15d3-120">Name</span></span>       | <span data-ttu-id="b15d3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b15d3-121">Type</span></span> | <span data-ttu-id="b15d3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b15d3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b15d3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b15d3-123">Authorization</span></span>  | <span data-ttu-id="b15d3-124">string</span><span class="sxs-lookup"><span data-stu-id="b15d3-124">string</span></span>  | <span data-ttu-id="b15d3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b15d3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b15d3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b15d3-127">Request body</span></span>
<span data-ttu-id="b15d3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b15d3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b15d3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b15d3-129">Response</span></span>
<span data-ttu-id="b15d3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b15d3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b15d3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b15d3-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b15d3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b15d3-133">Request</span></span>
<span data-ttu-id="b15d3-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b15d3-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b15d3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b15d3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="b15d3-136">C#</span><span class="sxs-lookup"><span data-stu-id="b15d3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b15d3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b15d3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b15d3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b15d3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b15d3-139">Java</span><span class="sxs-lookup"><span data-stu-id="b15d3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b15d3-140">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="b15d3-140">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="b15d3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b15d3-141">Response</span></span>
<span data-ttu-id="b15d3-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b15d3-142">The following is an example of the response.</span></span>
><span data-ttu-id="b15d3-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b15d3-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

