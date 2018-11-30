---
title: Excluir um usuário
description: Excluir usuário.
ms.openlocfilehash: f7f72ae91c636ef005768c2c4933ed2786ced91d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038668"
---
# <a name="delete-a-user"></a><span data-ttu-id="72006-103">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="72006-103">Delete a user</span></span>

> <span data-ttu-id="72006-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="72006-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72006-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="72006-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72006-106">Excluir usuário.</span><span class="sxs-lookup"><span data-stu-id="72006-106">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="72006-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="72006-107">Permissions</span></span>
<span data-ttu-id="72006-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72006-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72006-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72006-110">Permission type</span></span>      | <span data-ttu-id="72006-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72006-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72006-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72006-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72006-113">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="72006-113">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="72006-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72006-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72006-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72006-115">Not supported.</span></span>    |
|<span data-ttu-id="72006-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72006-116">Application</span></span> | <span data-ttu-id="72006-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72006-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72006-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72006-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="72006-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72006-119">Request headers</span></span>
| <span data-ttu-id="72006-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72006-120">Header</span></span>       | <span data-ttu-id="72006-121">Valor</span><span class="sxs-lookup"><span data-stu-id="72006-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="72006-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="72006-122">Authorization</span></span>  | <span data-ttu-id="72006-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72006-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72006-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72006-125">Request body</span></span>
<span data-ttu-id="72006-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72006-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72006-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="72006-127">Response</span></span>

<span data-ttu-id="72006-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72006-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72006-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72006-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72006-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72006-131">Request</span></span>
<span data-ttu-id="72006-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72006-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
##### <a name="response"></a><span data-ttu-id="72006-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="72006-133">Response</span></span>
<span data-ttu-id="72006-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72006-134">Here is an example of the response.</span></span> 
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