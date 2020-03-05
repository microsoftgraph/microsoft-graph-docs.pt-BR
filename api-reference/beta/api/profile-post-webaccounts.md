---
title: Criar conta da
description: Criar um novo objeto webaccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 36c519f1d6fa3f7236eafe9a005e3e80451a9a0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455043"
---
# <a name="create-webaccount"></a><span data-ttu-id="d8f2d-103">Criar conta da</span><span class="sxs-lookup"><span data-stu-id="d8f2d-103">Create webAccount</span></span>

<span data-ttu-id="d8f2d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d8f2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8f2d-105">Criar um novo objeto [webaccount](../resources/webaccount.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d8f2d-105">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8f2d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8f2d-106">Permissions</span></span>

<span data-ttu-id="d8f2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8f2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8f2d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8f2d-109">Permission type</span></span>                        | <span data-ttu-id="d8f2d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8f2d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d8f2d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8f2d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8f2d-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d8f2d-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d8f2d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8f2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8f2d-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d8f2d-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d8f2d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8f2d-115">Application</span></span>                            | <span data-ttu-id="d8f2d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8f2d-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8f2d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8f2d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="d8f2d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f2d-118">Request headers</span></span>

| <span data-ttu-id="d8f2d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d8f2d-119">Name</span></span>      |<span data-ttu-id="d8f2d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8f2d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d8f2d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8f2d-121">Authorization</span></span>  | <span data-ttu-id="d8f2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8f2d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d8f2d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8f2d-124">Content-Type</span></span>   | <span data-ttu-id="d8f2d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8f2d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8f2d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f2d-127">Request body</span></span>

<span data-ttu-id="d8f2d-128">No corpo da solicitação, forneça uma representação JSON do objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="d8f2d-128">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d8f2d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8f2d-129">Response</span></span>

<span data-ttu-id="d8f2d-130">Se bem-sucedido, este método retorna `201, Created` o código de resposta e um novo objeto [webaccount](../resources/webaccount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8f2d-130">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8f2d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d8f2d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8f2d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f2d-132">Request</span></span>

<span data-ttu-id="d8f2d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8f2d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8f2d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8f2d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_webaccount_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/webAccounts
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d8f2d-135">C#</span><span class="sxs-lookup"><span data-stu-id="d8f2d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8f2d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8f2d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8f2d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8f2d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d8f2d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8f2d-138">Response</span></span>

<span data-ttu-id="d8f2d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8f2d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="d8f2d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8f2d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create webAccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
