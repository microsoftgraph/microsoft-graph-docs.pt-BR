---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0cf8a6f58439a6bcd7c6605503b8c4d471d9f188
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181424"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="9778d-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="9778d-103">Remove directory role member</span></span>

<span data-ttu-id="9778d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9778d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9778d-105">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="9778d-105">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="9778d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9778d-106">Permissions</span></span>

<span data-ttu-id="9778d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9778d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9778d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9778d-109">Permission type</span></span>      | <span data-ttu-id="9778d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9778d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9778d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9778d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9778d-112">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="9778d-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9778d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9778d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9778d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9778d-114">Not supported.</span></span>    |
|<span data-ttu-id="9778d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9778d-115">Application</span></span> | <span data-ttu-id="9778d-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9778d-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="9778d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9778d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9778d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9778d-118">Request headers</span></span>

| <span data-ttu-id="9778d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9778d-119">Name</span></span>       | <span data-ttu-id="9778d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9778d-120">Type</span></span> | <span data-ttu-id="9778d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9778d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9778d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9778d-122">Authorization</span></span>  | <span data-ttu-id="9778d-123">string</span><span class="sxs-lookup"><span data-stu-id="9778d-123">string</span></span>  | <span data-ttu-id="9778d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9778d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9778d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9778d-126">Request body</span></span>

<span data-ttu-id="9778d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9778d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9778d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9778d-128">Response</span></span>

<span data-ttu-id="9778d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9778d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9778d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9778d-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9778d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9778d-132">Request</span></span>

<span data-ttu-id="9778d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9778d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9778d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9778d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="9778d-135">C#</span><span class="sxs-lookup"><span data-stu-id="9778d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9778d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9778d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9778d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9778d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9778d-138">Java</span><span class="sxs-lookup"><span data-stu-id="9778d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9778d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9778d-139">Response</span></span>

<span data-ttu-id="9778d-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9778d-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
