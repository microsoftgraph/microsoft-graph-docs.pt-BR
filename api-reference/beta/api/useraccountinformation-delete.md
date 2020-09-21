---
title: Excluir userAccountInformation
description: Excluir um objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b7df1498260be758fd7c945fe013b09d09e1aed0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050294"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="be1f8-103">Excluir userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="be1f8-103">Delete userAccountInformation</span></span>

<span data-ttu-id="be1f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be1f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be1f8-105">Excluir um objeto [userAccountInformation](../resources/useraccountinformation.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="be1f8-105">Delete an [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be1f8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be1f8-106">Permissions</span></span>

<span data-ttu-id="be1f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be1f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be1f8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be1f8-109">Permission type</span></span>                        | <span data-ttu-id="be1f8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be1f8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be1f8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be1f8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be1f8-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="be1f8-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="be1f8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be1f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be1f8-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="be1f8-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="be1f8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be1f8-115">Application</span></span>                            | <span data-ttu-id="be1f8-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be1f8-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="be1f8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be1f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/accounts/{id}
DELETE /users/{id | userPrincipalName}/profile/accounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="be1f8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be1f8-118">Request headers</span></span>

| <span data-ttu-id="be1f8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="be1f8-119">Name</span></span>           | <span data-ttu-id="be1f8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="be1f8-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="be1f8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="be1f8-121">Authorization</span></span>  | <span data-ttu-id="be1f8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be1f8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be1f8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be1f8-124">Request body</span></span>

<span data-ttu-id="be1f8-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be1f8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be1f8-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="be1f8-126">Response</span></span>

<span data-ttu-id="be1f8-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be1f8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be1f8-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be1f8-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be1f8-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be1f8-130">Request</span></span>

<span data-ttu-id="be1f8-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be1f8-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/accounts/{id}
```

### <a name="response"></a><span data-ttu-id="be1f8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="be1f8-132">Response</span></span>

<span data-ttu-id="be1f8-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be1f8-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

