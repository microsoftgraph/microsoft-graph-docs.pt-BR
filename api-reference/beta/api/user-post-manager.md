---
title: Atribuir um gerente
description: Use essa API para atribuir um gerente ao usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99a8725da3fe370b681e703673808601e8704b8d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866813"
---
# <a name="assign-a-manager"></a><span data-ttu-id="172bc-103">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="172bc-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="172bc-104">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="172bc-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="172bc-105">Observação: não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="172bc-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="172bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="172bc-106">Permissions</span></span>
<span data-ttu-id="172bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="172bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="172bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="172bc-109">Permission type</span></span>      | <span data-ttu-id="172bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="172bc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="172bc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="172bc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="172bc-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="172bc-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="172bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="172bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="172bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="172bc-114">Not supported.</span></span>    |
|<span data-ttu-id="172bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="172bc-115">Application</span></span> | <span data-ttu-id="172bc-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="172bc-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="172bc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="172bc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="172bc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="172bc-118">Request headers</span></span>
| <span data-ttu-id="172bc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="172bc-119">Name</span></span>       | <span data-ttu-id="172bc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="172bc-120">Type</span></span> | <span data-ttu-id="172bc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="172bc-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="172bc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="172bc-122">Authorization</span></span>  | <span data-ttu-id="172bc-123">string</span><span class="sxs-lookup"><span data-stu-id="172bc-123">string</span></span>  | <span data-ttu-id="172bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="172bc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="172bc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="172bc-126">Request body</span></span>
<span data-ttu-id="172bc-127">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="172bc-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="172bc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="172bc-128">Response</span></span>

<span data-ttu-id="172bc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="172bc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="172bc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="172bc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="172bc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="172bc-132">Request</span></span>
<span data-ttu-id="172bc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="172bc-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="172bc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="172bc-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="172bc-135">C#</span><span class="sxs-lookup"><span data-stu-id="172bc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-for-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="172bc-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="172bc-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-for-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="172bc-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="172bc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-for-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="172bc-138">Java</span><span class="sxs-lookup"><span data-stu-id="172bc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-for-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="172bc-139">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="172bc-139">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="172bc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="172bc-140">Response</span></span>
<span data-ttu-id="172bc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="172bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
