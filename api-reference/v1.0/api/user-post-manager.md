---
title: Atribuir gerente
description: Atribuir o gerente de um usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 36b24ef7b6e9fb7a35be3c87723b650581ec982c
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621445"
---
# <a name="assign-manager"></a><span data-ttu-id="67f3c-103">Atribuir gerente</span><span class="sxs-lookup"><span data-stu-id="67f3c-103">Assign manager</span></span>

<span data-ttu-id="67f3c-104">Atribuir o gerente de um usuário.</span><span class="sxs-lookup"><span data-stu-id="67f3c-104">Assign a user's manager.</span></span>
> [!NOTE]
> <span data-ttu-id="67f3c-105">Não é possível atribuir subordinados diretos; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="67f3c-105">You cannot assign direct reports; instead, use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="67f3c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="67f3c-106">Permissions</span></span>
<span data-ttu-id="67f3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67f3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67f3c-109">Permission type</span></span>      | <span data-ttu-id="67f3c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67f3c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67f3c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67f3c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67f3c-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67f3c-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67f3c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67f3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67f3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67f3c-114">Not supported.</span></span>    |
|<span data-ttu-id="67f3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67f3c-115">Application</span></span> | <span data-ttu-id="67f3c-116">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67f3c-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67f3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67f3c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="67f3c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67f3c-118">Request headers</span></span>
| <span data-ttu-id="67f3c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67f3c-119">Header</span></span>       | <span data-ttu-id="67f3c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="67f3c-120">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="67f3c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="67f3c-121">Authorization</span></span>  | <span data-ttu-id="67f3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67f3c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67f3c-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="67f3c-124">Content-type</span></span>   | <span data-ttu-id="67f3c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67f3c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67f3c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67f3c-127">Request body</span></span>
<span data-ttu-id="67f3c-128">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md), [User](../resources/user.md)ou [Contact organizacional](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="67f3c-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="67f3c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f3c-129">Response</span></span>

<span data-ttu-id="67f3c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67f3c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67f3c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67f3c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67f3c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67f3c-133">Request</span></span>
<span data-ttu-id="67f3c-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67f3c-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="67f3c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="67f3c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_manager_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67f3c-136">C#</span><span class="sxs-lookup"><span data-stu-id="67f3c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67f3c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67f3c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67f3c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67f3c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="67f3c-139">Java</span><span class="sxs-lookup"><span data-stu-id="67f3c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67f3c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f3c-140">Response</span></span>
<span data-ttu-id="67f3c-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67f3c-141">The following is an example of the response.</span></span>
><span data-ttu-id="67f3c-142">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="67f3c-142">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
