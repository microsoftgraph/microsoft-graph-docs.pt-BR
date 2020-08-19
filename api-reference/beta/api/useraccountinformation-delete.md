---
title: Excluir userAccountInformation
description: Excluir um objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 424eb7d8fd90a5f3ac25263d985be84d526051eb
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809198"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="3c820-103">Excluir userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="3c820-103">Delete userAccountInformation</span></span>

<span data-ttu-id="3c820-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c820-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c820-105">Excluir um objeto [userAccountInformation](../resources/useraccountinformation.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3c820-105">Delete an [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c820-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c820-106">Permissions</span></span>

<span data-ttu-id="3c820-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c820-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c820-109">Permission type</span></span>                        | <span data-ttu-id="3c820-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c820-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3c820-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c820-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c820-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3c820-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3c820-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c820-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c820-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3c820-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3c820-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c820-115">Application</span></span>                            | <span data-ttu-id="3c820-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c820-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3c820-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c820-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/accounts/{id}
DELETE /users/{id | userPrincipalName}/profile/accounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3c820-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c820-118">Request headers</span></span>

| <span data-ttu-id="3c820-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3c820-119">Name</span></span>           | <span data-ttu-id="3c820-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c820-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="3c820-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c820-121">Authorization</span></span>  | <span data-ttu-id="3c820-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c820-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c820-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c820-124">Request body</span></span>

<span data-ttu-id="3c820-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c820-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c820-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c820-126">Response</span></span>

<span data-ttu-id="3c820-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c820-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c820-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3c820-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c820-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c820-130">Request</span></span>

<span data-ttu-id="3c820-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c820-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/accounts/{id}
```

### <a name="response"></a><span data-ttu-id="3c820-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c820-132">Response</span></span>

<span data-ttu-id="3c820-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c820-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```