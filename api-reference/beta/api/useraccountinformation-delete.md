---
title: Excluir userAccountInformation
description: Excluir um objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 583184860730adbd64899bdc5091c40534677529
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228363"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="36b98-103">Excluir userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="36b98-103">Delete userAccountInformation</span></span>

<span data-ttu-id="36b98-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36b98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36b98-105">Excluir um objeto [userAccountInformation](../resources/useraccountinformation.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="36b98-105">Delete a [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="36b98-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36b98-106">Permissions</span></span>

<span data-ttu-id="36b98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36b98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36b98-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36b98-109">Permission type</span></span>                        | <span data-ttu-id="36b98-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36b98-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36b98-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36b98-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36b98-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36b98-112">Not supported.</span></span>                              |
| <span data-ttu-id="36b98-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36b98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36b98-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36b98-114">Not supported.</span></span>                              |
| <span data-ttu-id="36b98-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36b98-115">Application</span></span>                            | <span data-ttu-id="36b98-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36b98-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="36b98-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36b98-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /user/profile/account{id}
```

## <a name="request-headers"></a><span data-ttu-id="36b98-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36b98-118">Request headers</span></span>

| <span data-ttu-id="36b98-119">Nome</span><span class="sxs-lookup"><span data-stu-id="36b98-119">Name</span></span>           | <span data-ttu-id="36b98-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="36b98-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="36b98-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="36b98-121">Authorization</span></span>  | <span data-ttu-id="36b98-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36b98-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36b98-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36b98-124">Request body</span></span>

<span data-ttu-id="36b98-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36b98-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36b98-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="36b98-126">Response</span></span>

<span data-ttu-id="36b98-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36b98-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36b98-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36b98-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36b98-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36b98-130">Request</span></span>

<span data-ttu-id="36b98-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36b98-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="36b98-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="36b98-132">Response</span></span>

<span data-ttu-id="36b98-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36b98-133">The following is an example of the response.</span></span>

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
  "description": "Delete userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
