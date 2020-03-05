---
title: Criar personWebsite
description: Criar um novo personWebsite.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9fee97962e998a010dd4bbf57b9a9e9c4a766296
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455057"
---
# <a name="create-personwebsite"></a><span data-ttu-id="cce2f-103">Criar personWebsite</span><span class="sxs-lookup"><span data-stu-id="cce2f-103">Create personWebsite</span></span>

<span data-ttu-id="cce2f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cce2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cce2f-105">Criar um novo objeto [personWebsite](../resources/personwebsite.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="cce2f-105">Create a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cce2f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cce2f-106">Permissions</span></span>

<span data-ttu-id="cce2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cce2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cce2f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cce2f-109">Permission type</span></span>                        | <span data-ttu-id="cce2f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cce2f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cce2f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cce2f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cce2f-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cce2f-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cce2f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cce2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cce2f-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cce2f-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cce2f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cce2f-115">Application</span></span>                            | <span data-ttu-id="cce2f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cce2f-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cce2f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cce2f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/websites
```

## <a name="request-headers"></a><span data-ttu-id="cce2f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cce2f-118">Request headers</span></span>

| <span data-ttu-id="cce2f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cce2f-119">Name</span></span>      |<span data-ttu-id="cce2f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cce2f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cce2f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cce2f-121">Authorization</span></span>  | <span data-ttu-id="cce2f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cce2f-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cce2f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cce2f-124">Content-Type</span></span>   | <span data-ttu-id="cce2f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cce2f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cce2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cce2f-127">Request body</span></span>

<span data-ttu-id="cce2f-128">No corpo da solicitação, forneça uma representação JSON do objeto [personWebsite](../resources/personwebsite.md) .</span><span class="sxs-lookup"><span data-stu-id="cce2f-128">In the request body, supply a JSON representation of [personWebsite](../resources/personwebsite.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cce2f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cce2f-129">Response</span></span>

<span data-ttu-id="cce2f-130">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [personWebsite](../resources/personwebsite.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cce2f-130">If successful, this method returns `201, Created` response code and a new [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cce2f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cce2f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cce2f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cce2f-132">Request</span></span>

<span data-ttu-id="cce2f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cce2f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cce2f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cce2f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personwebsite_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/websites
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="cce2f-135">C#</span><span class="sxs-lookup"><span data-stu-id="cce2f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personwebsite-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cce2f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cce2f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personwebsite-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cce2f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cce2f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personwebsite-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cce2f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cce2f-138">Response</span></span>

<span data-ttu-id="cce2f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cce2f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="cce2f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cce2f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personWebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
