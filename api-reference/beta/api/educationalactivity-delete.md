---
title: Excluir educationalActivity
description: Excluir um objeto educationalActivity de um perfil de usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 96c717171f683d2a32e62b4e79b80639e2cb5242
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810948"
---
# <a name="delete-educationalactivity"></a><span data-ttu-id="4b598-103">Excluir educationalActivity</span><span class="sxs-lookup"><span data-stu-id="4b598-103">Delete educationalActivity</span></span>

<span data-ttu-id="4b598-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b598-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b598-105">Excluir um objeto [educationalActivity](../resources/educationalactivity.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b598-105">Delete an [educationalActivity](../resources/educationalactivity.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b598-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b598-106">Permissions</span></span>

<span data-ttu-id="4b598-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b598-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b598-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b598-109">Permission type</span></span>                        | <span data-ttu-id="4b598-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b598-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b598-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b598-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b598-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4b598-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4b598-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b598-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b598-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4b598-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4b598-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b598-115">Application</span></span>                            | <span data-ttu-id="4b598-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b598-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4b598-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b598-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/educationalActivities/{id} 
DELETE /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4b598-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b598-118">Request headers</span></span>

| <span data-ttu-id="4b598-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4b598-119">Name</span></span>           |<span data-ttu-id="4b598-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b598-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4b598-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b598-121">Authorization</span></span>  | <span data-ttu-id="4b598-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b598-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="4b598-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b598-124">Request body</span></span>

<span data-ttu-id="4b598-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b598-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b598-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b598-126">Response</span></span>

<span data-ttu-id="4b598-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b598-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b598-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4b598-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b598-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b598-130">Request</span></span>

<span data-ttu-id="4b598-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b598-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationalactivity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```

### <a name="response"></a><span data-ttu-id="4b598-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b598-132">Response</span></span>

<span data-ttu-id="4b598-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4b598-133">The following is an example of the response.</span></span>

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
