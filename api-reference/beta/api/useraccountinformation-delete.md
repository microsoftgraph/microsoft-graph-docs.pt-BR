---
title: Excluir userAccountInformation
description: Excluir um objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1cd1130b89104f1154425e94443a45e375012a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451578"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="98599-103">Excluir userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="98599-103">Delete userAccountInformation</span></span>

<span data-ttu-id="98599-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="98599-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98599-105">Excluir um objeto [userAccountInformation](../resources/useraccountinformation.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="98599-105">Delete a [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="98599-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="98599-106">Permissions</span></span>

<span data-ttu-id="98599-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98599-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98599-109">Permission type</span></span>                        | <span data-ttu-id="98599-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98599-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98599-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98599-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="98599-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98599-112">Not supported.</span></span>                              |
| <span data-ttu-id="98599-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98599-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98599-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98599-114">Not supported.</span></span>                              |
| <span data-ttu-id="98599-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98599-115">Application</span></span>                            | <span data-ttu-id="98599-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98599-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="98599-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98599-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /user/profile/account{id}
```

## <a name="request-headers"></a><span data-ttu-id="98599-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98599-118">Request headers</span></span>

| <span data-ttu-id="98599-119">Nome</span><span class="sxs-lookup"><span data-stu-id="98599-119">Name</span></span>           |<span data-ttu-id="98599-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="98599-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="98599-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="98599-121">Authorization</span></span>  | <span data-ttu-id="98599-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98599-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98599-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98599-124">Request body</span></span>

<span data-ttu-id="98599-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98599-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98599-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="98599-126">Response</span></span>

<span data-ttu-id="98599-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98599-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98599-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="98599-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98599-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98599-130">Request</span></span>

<span data-ttu-id="98599-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="98599-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="98599-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="98599-132">Response</span></span>

<span data-ttu-id="98599-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="98599-133">The following is an example of the response.</span></span>

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
