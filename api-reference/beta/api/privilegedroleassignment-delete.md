---
title: Delete privilegedRoleAssignment
description: Exclua privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: d6779a2cfa23cb9f947045b8c7370094790c8a10
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268156"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="d1abc-103">Delete privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d1abc-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1abc-104">Exclua [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d1abc-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d1abc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1abc-105">Permissions</span></span>
<span data-ttu-id="d1abc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d1abc-108">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="d1abc-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="d1abc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1abc-109">Permission type</span></span>      | <span data-ttu-id="d1abc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1abc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1abc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1abc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d1abc-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d1abc-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d1abc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1abc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1abc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1abc-114">Not supported.</span></span>    |
|<span data-ttu-id="d1abc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1abc-115">Application</span></span> | <span data-ttu-id="d1abc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1abc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1abc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1abc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="d1abc-118">Observe que ``<id>`` está no formato de ' userId_roleId ', onde userid é a cadeia de caracteres GUID da ID de usuário do Azure AD e RoleID é a cadeia de caracteres GUID da ID da função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="d1abc-118">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1abc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1abc-119">Request headers</span></span>
| <span data-ttu-id="d1abc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d1abc-120">Name</span></span>       | <span data-ttu-id="d1abc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1abc-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1abc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1abc-122">Authorization</span></span>  | <span data-ttu-id="d1abc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1abc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1abc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1abc-125">Request body</span></span>
<span data-ttu-id="d1abc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1abc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1abc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1abc-127">Response</span></span>

<span data-ttu-id="d1abc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1abc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="d1abc-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="d1abc-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d1abc-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="d1abc-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d1abc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1abc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1abc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1abc-133">Request</span></span>
<span data-ttu-id="d1abc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1abc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="d1abc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1abc-135">Response</span></span>
<span data-ttu-id="d1abc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1abc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1abc-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d1abc-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1abc-140">C#</span><span class="sxs-lookup"><span data-stu-id="d1abc-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_privilegedroleassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1abc-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1abc-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_privilegedroleassignment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d1abc-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d1abc-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_privilegedroleassignment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
