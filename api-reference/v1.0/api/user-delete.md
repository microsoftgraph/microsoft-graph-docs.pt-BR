---
title: Excluir um usuário
description: Excluir usuário.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: c7cbdf08b8bf18d393dd8e388c4d6de9f7fbf407
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875688"
---
# <a name="delete-a-user"></a><span data-ttu-id="d4f2d-103">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="d4f2d-103">Delete a user</span></span>

<span data-ttu-id="d4f2d-104">Excluir usuário.</span><span class="sxs-lookup"><span data-stu-id="d4f2d-104">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="d4f2d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4f2d-105">Permissions</span></span>
<span data-ttu-id="d4f2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4f2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4f2d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4f2d-108">Permission type</span></span>      | <span data-ttu-id="d4f2d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4f2d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4f2d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4f2d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4f2d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4f2d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4f2d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4f2d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4f2d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4f2d-113">Not supported.</span></span>    |
|<span data-ttu-id="d4f2d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4f2d-114">Application</span></span> | <span data-ttu-id="d4f2d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4f2d-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4f2d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4f2d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="d4f2d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f2d-117">Request headers</span></span>
| <span data-ttu-id="d4f2d-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4f2d-118">Header</span></span>       | <span data-ttu-id="d4f2d-119">Valor</span><span class="sxs-lookup"><span data-stu-id="d4f2d-119">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d4f2d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4f2d-120">Authorization</span></span>  | <span data-ttu-id="d4f2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4f2d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4f2d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f2d-123">Request body</span></span>
<span data-ttu-id="d4f2d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4f2d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4f2d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4f2d-125">Response</span></span>

<span data-ttu-id="d4f2d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4f2d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4f2d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4f2d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4f2d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f2d-129">Request</span></span>
<span data-ttu-id="d4f2d-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4f2d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="d4f2d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4f2d-131">Response</span></span>
<span data-ttu-id="d4f2d-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4f2d-132">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
