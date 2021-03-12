---
title: Atribuir gerente
description: Atribuir um gerenciador de usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 34ffe0a968ef500214d7f987d3a76c7fe4616cf7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721415"
---
# <a name="assign-manager"></a><span data-ttu-id="bf00a-103">Atribuir gerente</span><span class="sxs-lookup"><span data-stu-id="bf00a-103">Assign manager</span></span>

<span data-ttu-id="bf00a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf00a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf00a-105">Atribuir um gerenciador de usuário.</span><span class="sxs-lookup"><span data-stu-id="bf00a-105">Assign a user's manager.</span></span>
> [!NOTE]
> <span data-ttu-id="bf00a-106">Não é possível atribuir relatórios diretos; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="bf00a-106">You cannot assign direct reports; instead, use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf00a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="bf00a-107">Permissions</span></span>
<span data-ttu-id="bf00a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf00a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf00a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf00a-110">Permission type</span></span>      | <span data-ttu-id="bf00a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf00a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf00a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf00a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf00a-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf00a-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf00a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf00a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf00a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf00a-115">Not supported.</span></span>    |
|<span data-ttu-id="bf00a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf00a-116">Application</span></span> | <span data-ttu-id="bf00a-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf00a-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf00a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf00a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bf00a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf00a-119">Request headers</span></span>
| <span data-ttu-id="bf00a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf00a-120">Header</span></span>       | <span data-ttu-id="bf00a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bf00a-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bf00a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf00a-122">Authorization</span></span>  | <span data-ttu-id="bf00a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf00a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf00a-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="bf00a-125">Content-type</span></span>   | <span data-ttu-id="bf00a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf00a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf00a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf00a-128">Request body</span></span>
<span data-ttu-id="bf00a-129">No corpo da solicitação, fornece uma representação JSON de um objeto de contato [directoryObject](../resources/directoryobject.md), [usuário](../resources/user.md)ou [organizacional](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="bf00a-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="bf00a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf00a-130">Response</span></span>

<span data-ttu-id="bf00a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf00a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf00a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf00a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf00a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf00a-134">Request</span></span>
<span data-ttu-id="bf00a-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf00a-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf00a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf00a-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bf00a-137">C#</span><span class="sxs-lookup"><span data-stu-id="bf00a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf00a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf00a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf00a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf00a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf00a-140">Java</span><span class="sxs-lookup"><span data-stu-id="bf00a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bf00a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf00a-141">Response</span></span>
<span data-ttu-id="bf00a-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bf00a-142">The following is an example of the response.</span></span>
><span data-ttu-id="bf00a-143">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bf00a-143">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

