---
title: Excluir um usuário - Microsoft Graph API
description: Descreve o método de exclusão de recursos do usuário (entidade) do Microsoft Graph API (REST).
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba27c81e5cb6b8bc8738c419b467e686932bc7c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567911"
---
# <a name="delete-a-user"></a><span data-ttu-id="d36e3-103">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="d36e3-103">Delete a user</span></span>

<span data-ttu-id="d36e3-104">Excluir usuário.</span><span class="sxs-lookup"><span data-stu-id="d36e3-104">Delete user.</span></span>  

<span data-ttu-id="d36e3-105">Quando excluído, os recursos do usuário são movidos para um contêiner temporário e poderá ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="d36e3-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="d36e3-106">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="d36e3-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="d36e3-107">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="d36e3-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d36e3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d36e3-108">Permissions</span></span>

<span data-ttu-id="d36e3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d36e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d36e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d36e3-111">Permission type</span></span>      | <span data-ttu-id="d36e3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d36e3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d36e3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d36e3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d36e3-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d36e3-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d36e3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d36e3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d36e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d36e3-116">Not supported.</span></span>    |
|<span data-ttu-id="d36e3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d36e3-117">Application</span></span> | <span data-ttu-id="d36e3-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d36e3-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d36e3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d36e3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="d36e3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d36e3-120">Request headers</span></span>

| <span data-ttu-id="d36e3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d36e3-121">Header</span></span>       | <span data-ttu-id="d36e3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d36e3-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d36e3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d36e3-123">Authorization</span></span>  | <span data-ttu-id="d36e3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d36e3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d36e3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d36e3-126">Request body</span></span>

<span data-ttu-id="d36e3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d36e3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d36e3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d36e3-128">Response</span></span>

<span data-ttu-id="d36e3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d36e3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d36e3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d36e3-131">Example</span></span>

## <a name="request"></a><span data-ttu-id="d36e3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d36e3-132">Request</span></span>

<span data-ttu-id="d36e3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d36e3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
### <a name="response"></a><span data-ttu-id="d36e3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d36e3-134">Response</span></span>

<span data-ttu-id="d36e3-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d36e3-135">Here is an example of the response.</span></span> 
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
