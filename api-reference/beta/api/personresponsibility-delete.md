---
title: Excluir personResponsibility
description: Exclui um objeto personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bb99620a23370f6763fa6544a3992053f5057183
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812881"
---
# <a name="delete-personresponsibility"></a><span data-ttu-id="417e9-103">Excluir personResponsibility</span><span class="sxs-lookup"><span data-stu-id="417e9-103">Delete personResponsibility</span></span>
<span data-ttu-id="417e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="417e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="417e9-105">Exclui um objeto [personResponsibility](../resources/personresponsibility.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="417e9-105">Deletes a [personResponsibility](../resources/personresponsibility.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="417e9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="417e9-106">Permissions</span></span>

<span data-ttu-id="417e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="417e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="417e9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="417e9-109">Permission type</span></span>                        | <span data-ttu-id="417e9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="417e9-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="417e9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="417e9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="417e9-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="417e9-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="417e9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="417e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="417e9-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="417e9-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="417e9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="417e9-115">Application</span></span>                            | <span data-ttu-id="417e9-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="417e9-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="417e9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="417e9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/responsibilities/{id}
DELETE /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="417e9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="417e9-118">Request headers</span></span>
|<span data-ttu-id="417e9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="417e9-119">Name</span></span>|<span data-ttu-id="417e9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="417e9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="417e9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="417e9-121">Authorization</span></span>|<span data-ttu-id="417e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="417e9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="417e9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="417e9-124">Request body</span></span>
<span data-ttu-id="417e9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="417e9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="417e9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="417e9-126">Response</span></span>

<span data-ttu-id="417e9-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="417e9-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="417e9-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="417e9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="417e9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="417e9-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "delete_personresponsibility"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="417e9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="417e9-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
