---
title: Atribuir um gerente
description: Use essa API para atribuir um gerente ao usuário.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 00350bc85bb7e3952fe06dde424a3a8c83ee7e34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064532"
---
# <a name="assign-a-manager"></a><span data-ttu-id="81122-103">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="81122-103">Assign a manager</span></span>

<span data-ttu-id="81122-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81122-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81122-105">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="81122-105">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="81122-106">Observação: não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="81122-106">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="81122-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="81122-107">Permissions</span></span>
<span data-ttu-id="81122-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81122-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81122-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81122-110">Permission type</span></span>      | <span data-ttu-id="81122-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81122-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81122-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81122-112">Delegated (work or school account)</span></span> | <span data-ttu-id="81122-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81122-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81122-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81122-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81122-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81122-115">Not supported.</span></span>    |
|<span data-ttu-id="81122-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81122-116">Application</span></span> | <span data-ttu-id="81122-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81122-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81122-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81122-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="81122-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81122-119">Request headers</span></span>
| <span data-ttu-id="81122-120">Nome</span><span class="sxs-lookup"><span data-stu-id="81122-120">Name</span></span>       | <span data-ttu-id="81122-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="81122-121">Type</span></span> | <span data-ttu-id="81122-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="81122-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81122-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81122-123">Authorization</span></span>  | <span data-ttu-id="81122-124">string</span><span class="sxs-lookup"><span data-stu-id="81122-124">string</span></span>  | <span data-ttu-id="81122-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81122-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81122-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81122-127">Request body</span></span>
<span data-ttu-id="81122-128">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="81122-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="81122-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="81122-129">Response</span></span>

<span data-ttu-id="81122-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81122-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81122-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81122-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81122-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81122-133">Request</span></span>
<span data-ttu-id="81122-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81122-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81122-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="81122-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_manager_for_user"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="81122-136">C#</span><span class="sxs-lookup"><span data-stu-id="81122-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-for-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81122-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81122-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-for-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81122-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81122-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-for-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81122-139">Java</span><span class="sxs-lookup"><span data-stu-id="81122-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-for-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="81122-140">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="81122-140">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="81122-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="81122-141">Response</span></span>
<span data-ttu-id="81122-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81122-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


