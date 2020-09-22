---
title: Atribuir gerente
description: Atribuir um gerenciador de usuário.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 20c4a97c183fc3109721c600a41e16f7b704fbb2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972698"
---
# <a name="assign-manager"></a><span data-ttu-id="5566f-103">Atribuir gerente</span><span class="sxs-lookup"><span data-stu-id="5566f-103">Assign manager</span></span>

<span data-ttu-id="5566f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5566f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5566f-105">Atribuir um gerenciador de usuário.</span><span class="sxs-lookup"><span data-stu-id="5566f-105">Assign a user's manager.</span></span>
> [!NOTE]
> <span data-ttu-id="5566f-106">Não é possível atribuir subordinados diretos; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="5566f-106">You cannot assign direct reports; instead, use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="5566f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5566f-107">Permissions</span></span>
<span data-ttu-id="5566f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5566f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5566f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5566f-110">Permission type</span></span>      | <span data-ttu-id="5566f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5566f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5566f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5566f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5566f-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5566f-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5566f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5566f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5566f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5566f-115">Not supported.</span></span>    |
|<span data-ttu-id="5566f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5566f-116">Application</span></span> | <span data-ttu-id="5566f-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5566f-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5566f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5566f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5566f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5566f-119">Request headers</span></span>
| <span data-ttu-id="5566f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5566f-120">Header</span></span>       | <span data-ttu-id="5566f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5566f-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5566f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5566f-122">Authorization</span></span>  | <span data-ttu-id="5566f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5566f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5566f-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="5566f-125">Content-type</span></span>   | <span data-ttu-id="5566f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5566f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5566f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5566f-128">Request body</span></span>
<span data-ttu-id="5566f-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md), [User](../resources/user.md)ou [Contact organizacional](../resources/orgcontact.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="5566f-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="5566f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5566f-130">Response</span></span>

<span data-ttu-id="5566f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5566f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5566f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5566f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5566f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5566f-134">Request</span></span>
<span data-ttu-id="5566f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5566f-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5566f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5566f-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5566f-137">C#</span><span class="sxs-lookup"><span data-stu-id="5566f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5566f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5566f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5566f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5566f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5566f-140">Java</span><span class="sxs-lookup"><span data-stu-id="5566f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5566f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5566f-141">Response</span></span>
<span data-ttu-id="5566f-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5566f-142">The following is an example of the response.</span></span>
><span data-ttu-id="5566f-143">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5566f-143">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

