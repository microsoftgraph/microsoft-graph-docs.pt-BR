---
title: Delete privilegedRoleAssignment
description: Exclua privilegedRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a28842b23825db7b010e2d597d592f1fd5ec5db2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055236"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="c325f-103">Delete privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c325f-103">Delete privilegedRoleAssignment</span></span>

<span data-ttu-id="c325f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c325f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c325f-105">Excluir [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c325f-105">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c325f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c325f-106">Permissions</span></span>
<span data-ttu-id="c325f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c325f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c325f-109">O solicitante precisa ter função _de Administrador de Função_ Privilegiada.</span><span class="sxs-lookup"><span data-stu-id="c325f-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="c325f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c325f-110">Permission type</span></span>      | <span data-ttu-id="c325f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c325f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c325f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c325f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c325f-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c325f-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c325f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c325f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c325f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c325f-115">Not supported.</span></span>    |
|<span data-ttu-id="c325f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c325f-116">Application</span></span> | <span data-ttu-id="c325f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c325f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c325f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c325f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="c325f-119">Observe que está no formato de "userId_roleId", onde userId é a cadeia de caracteres GUID para id de usuário do Azure AD e roleId é a cadeia de caracteres GUID para id de função de administrador do ``{id}`` Azure.</span><span class="sxs-lookup"><span data-stu-id="c325f-119">Note that ``{id}`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c325f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c325f-120">Request headers</span></span>
| <span data-ttu-id="c325f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c325f-121">Name</span></span>       | <span data-ttu-id="c325f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c325f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c325f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c325f-123">Authorization</span></span>  | <span data-ttu-id="c325f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c325f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c325f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c325f-126">Request body</span></span>
<span data-ttu-id="c325f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c325f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c325f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c325f-128">Response</span></span>

<span data-ttu-id="c325f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c325f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="c325f-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="c325f-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c325f-132">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="c325f-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c325f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c325f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c325f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c325f-134">Request</span></span>
<span data-ttu-id="c325f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c325f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c325f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c325f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="c325f-137">C#</span><span class="sxs-lookup"><span data-stu-id="c325f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c325f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c325f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c325f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c325f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c325f-140">Java</span><span class="sxs-lookup"><span data-stu-id="c325f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-privilegedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c325f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c325f-141">Response</span></span>
<span data-ttu-id="c325f-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c325f-142">Here is an example of the response.</span></span> <span data-ttu-id="c325f-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c325f-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


