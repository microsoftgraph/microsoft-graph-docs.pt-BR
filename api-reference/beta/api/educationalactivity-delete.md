---
title: Excluir educationalActivity
description: Excluir um objeto educationalActivity de um perfil de usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b1c4a5069f192a481b9f4814115e3d6fcee6fc55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427897"
---
# <a name="delete-educationalactivity"></a><span data-ttu-id="724e3-103">Excluir educationalActivity</span><span class="sxs-lookup"><span data-stu-id="724e3-103">Delete educationalActivity</span></span>

<span data-ttu-id="724e3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="724e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="724e3-105">Excluir um objeto [educationalActivity](../resources/educationalactivity.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="724e3-105">Delete an [educationalActivity](../resources/educationalactivity.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="724e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="724e3-106">Permissions</span></span>

<span data-ttu-id="724e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="724e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="724e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="724e3-109">Permission type</span></span>                        | <span data-ttu-id="724e3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="724e3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="724e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="724e3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="724e3-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="724e3-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="724e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="724e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="724e3-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="724e3-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="724e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="724e3-115">Application</span></span>                            | <span data-ttu-id="724e3-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="724e3-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="724e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="724e3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="724e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="724e3-118">Request headers</span></span>

| <span data-ttu-id="724e3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="724e3-119">Name</span></span>           |<span data-ttu-id="724e3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="724e3-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="724e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="724e3-121">Authorization</span></span>  | <span data-ttu-id="724e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="724e3-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="724e3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="724e3-124">Request body</span></span>

<span data-ttu-id="724e3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="724e3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="724e3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="724e3-126">Response</span></span>

<span data-ttu-id="724e3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="724e3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="724e3-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="724e3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="724e3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="724e3-130">Request</span></span>

<span data-ttu-id="724e3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="724e3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationalactivity"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/educationalActivities/{id}
```

### <a name="response"></a><span data-ttu-id="724e3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="724e3-132">Response</span></span>

<span data-ttu-id="724e3-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="724e3-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
