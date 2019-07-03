---
title: Delete privilegedRoleAssignment
description: Exclua privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 76db67452db136d126774f2b7c93e372e7e582f2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444992"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="42766-103">Delete privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="42766-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42766-104">Exclua [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="42766-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="42766-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="42766-105">Permissions</span></span>
<span data-ttu-id="42766-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42766-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="42766-108">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="42766-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="42766-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42766-109">Permission type</span></span>      | <span data-ttu-id="42766-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42766-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42766-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42766-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42766-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42766-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42766-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42766-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42766-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42766-114">Not supported.</span></span>    |
|<span data-ttu-id="42766-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42766-115">Application</span></span> | <span data-ttu-id="42766-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42766-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42766-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42766-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="42766-118">Observe que ``<id>`` está no formato de ' userId_roleId ', onde userid é a cadeia de caracteres GUID da ID de usuário do Azure AD e RoleID é a cadeia de caracteres GUID da ID da função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="42766-118">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42766-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42766-119">Request headers</span></span>
| <span data-ttu-id="42766-120">Nome</span><span class="sxs-lookup"><span data-stu-id="42766-120">Name</span></span>       | <span data-ttu-id="42766-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="42766-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42766-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42766-122">Authorization</span></span>  | <span data-ttu-id="42766-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42766-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42766-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42766-125">Request body</span></span>
<span data-ttu-id="42766-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42766-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42766-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="42766-127">Response</span></span>

<span data-ttu-id="42766-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42766-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="42766-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="42766-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="42766-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="42766-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="42766-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42766-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42766-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42766-133">Request</span></span>
<span data-ttu-id="42766-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42766-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="42766-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="42766-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42766-136">C#</span><span class="sxs-lookup"><span data-stu-id="42766-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42766-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="42766-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42766-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="42766-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42766-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="42766-139">Response</span></span>
<span data-ttu-id="42766-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42766-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
