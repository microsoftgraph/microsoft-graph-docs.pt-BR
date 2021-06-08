---
title: Atribuir um gerente
description: Use essa API para atribuir um gerente ao usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e88a3ad02556ed14cc4aa7024c3414b36fa954a1
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785127"
---
# <a name="assign-a-manager"></a><span data-ttu-id="d14fd-103">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="d14fd-103">Assign a manager</span></span>

<span data-ttu-id="d14fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d14fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d14fd-105">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d14fd-105">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="d14fd-106">Observação: não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="d14fd-106">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="d14fd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d14fd-107">Permissions</span></span>
<span data-ttu-id="d14fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d14fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d14fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d14fd-110">Permission type</span></span>      | <span data-ttu-id="d14fd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d14fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d14fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d14fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d14fd-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d14fd-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d14fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d14fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d14fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d14fd-115">Not supported.</span></span>    |
|<span data-ttu-id="d14fd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d14fd-116">Application</span></span> | <span data-ttu-id="d14fd-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d14fd-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d14fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d14fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d14fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d14fd-119">Request headers</span></span>
| <span data-ttu-id="d14fd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d14fd-120">Name</span></span>       | <span data-ttu-id="d14fd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d14fd-121">Type</span></span> | <span data-ttu-id="d14fd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d14fd-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d14fd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d14fd-123">Authorization</span></span>  | <span data-ttu-id="d14fd-124">string</span><span class="sxs-lookup"><span data-stu-id="d14fd-124">string</span></span>  | <span data-ttu-id="d14fd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d14fd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d14fd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d14fd-127">Request body</span></span>
<span data-ttu-id="d14fd-128">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="d14fd-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d14fd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d14fd-129">Response</span></span>

<span data-ttu-id="d14fd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d14fd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d14fd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d14fd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d14fd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d14fd-133">Request</span></span>
<span data-ttu-id="d14fd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d14fd-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d14fd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d14fd-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d14fd-136">C#</span><span class="sxs-lookup"><span data-stu-id="d14fd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-for-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d14fd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d14fd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-for-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d14fd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d14fd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-for-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d14fd-139">Java</span><span class="sxs-lookup"><span data-stu-id="d14fd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-for-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d14fd-140">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="d14fd-140">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="d14fd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d14fd-141">Response</span></span>
<span data-ttu-id="d14fd-p104">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="d14fd-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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


