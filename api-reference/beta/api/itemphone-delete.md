---
title: Excluir o número de telefone
description: Excluir um objeto MyPhone do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0c7550f1b8e97fbc1a5efcc5d7e712f2550131a8
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808050"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="3b720-103">Excluir itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="3b720-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="3b720-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b720-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b720-105">Exclua um objeto [MyPhone](../resources/itemphone.md) do [perfil](../resources/profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="3b720-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b720-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b720-106">Permissions</span></span>

<span data-ttu-id="3b720-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b720-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b720-109">Permission type</span></span>                        | <span data-ttu-id="3b720-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b720-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3b720-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b720-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b720-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3b720-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3b720-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b720-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b720-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3b720-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3b720-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b720-115">Application</span></span>                            | <span data-ttu-id="3b720-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b720-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3b720-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b720-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/phones/{itemPhoneId}
DELETE /user/{userId}/profile/phones/{itemPhoneId}
```

## <a name="request-headers"></a><span data-ttu-id="3b720-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b720-118">Request headers</span></span>

|<span data-ttu-id="3b720-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3b720-119">Name</span></span>|<span data-ttu-id="3b720-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b720-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b720-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b720-121">Authorization</span></span>|<span data-ttu-id="3b720-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b720-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b720-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b720-124">Request body</span></span>

<span data-ttu-id="3b720-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b720-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b720-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b720-126">Response</span></span>

<span data-ttu-id="3b720-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3b720-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3b720-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3b720-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3b720-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b720-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/phones/{itemPhoneId}
```

### <a name="response"></a><span data-ttu-id="3b720-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b720-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
