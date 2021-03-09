---
title: Excluir itemPhone
description: Exclua um objeto itemPhone do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4b947a7674f73a4351cdb6742587812acd66d253
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577412"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="1098f-103">Excluir itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1098f-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="1098f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1098f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1098f-105">Excluir um [objeto itemPhone](../resources/itemphone.md) do perfil do [usuário](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="1098f-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1098f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1098f-106">Permissions</span></span>

<span data-ttu-id="1098f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1098f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1098f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1098f-109">Permission type</span></span>                        | <span data-ttu-id="1098f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1098f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1098f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1098f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1098f-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1098f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1098f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1098f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1098f-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1098f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1098f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1098f-115">Application</span></span>                            | <span data-ttu-id="1098f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1098f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1098f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1098f-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/phones/{itemPhoneId}
DELETE /users/{userId}/profile/phones/{itemPhoneId}
```

## <a name="request-headers"></a><span data-ttu-id="1098f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1098f-118">Request headers</span></span>

|<span data-ttu-id="1098f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1098f-119">Name</span></span>|<span data-ttu-id="1098f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1098f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1098f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1098f-121">Authorization</span></span>|<span data-ttu-id="1098f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1098f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1098f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1098f-124">Request body</span></span>

<span data-ttu-id="1098f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1098f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1098f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1098f-126">Response</span></span>

<span data-ttu-id="1098f-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1098f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1098f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1098f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1098f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1098f-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/phones/{itemPhoneId}
```

### <a name="response"></a><span data-ttu-id="1098f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1098f-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


