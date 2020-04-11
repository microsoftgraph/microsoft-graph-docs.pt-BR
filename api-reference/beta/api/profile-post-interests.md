---
title: Criar personInterest
description: Criar um novo personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: f0d4f406004d80121f2cd9ac44b39f303af71861
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229329"
---
# <a name="create-personinterest"></a><span data-ttu-id="1fc58-103">Criar personInterest</span><span class="sxs-lookup"><span data-stu-id="1fc58-103">Create personInterest</span></span>

<span data-ttu-id="1fc58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fc58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fc58-105">Criar um novo [personInterest] (.. /resources/personinterest.md].</span><span class="sxs-lookup"><span data-stu-id="1fc58-105">Create a new [personInterest](../resources/personinterest.md].</span></span>

## <a name="permissions"></a><span data-ttu-id="1fc58-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fc58-106">Permissions</span></span>

<span data-ttu-id="1fc58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fc58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fc58-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fc58-109">Permission type</span></span>                        | <span data-ttu-id="1fc58-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fc58-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1fc58-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fc58-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fc58-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1fc58-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1fc58-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fc58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fc58-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1fc58-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1fc58-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fc58-115">Application</span></span>                            | <span data-ttu-id="1fc58-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc58-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1fc58-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fc58-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="1fc58-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fc58-118">Request headers</span></span>

| <span data-ttu-id="1fc58-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1fc58-119">Name</span></span>      |<span data-ttu-id="1fc58-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fc58-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1fc58-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fc58-121">Authorization</span></span>  | <span data-ttu-id="1fc58-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fc58-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1fc58-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fc58-124">Content-Type</span></span>   | <span data-ttu-id="1fc58-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fc58-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fc58-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fc58-127">Request body</span></span>

<span data-ttu-id="1fc58-128">No corpo da solicitação, forneça uma representação JSON do objeto [personInterest](../resources/personinterest.md) .</span><span class="sxs-lookup"><span data-stu-id="1fc58-128">In the request body, supply a JSON representation of [personInterest](../resources/personinterest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1fc58-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fc58-129">Response</span></span>

<span data-ttu-id="1fc58-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [personInterest](../resources/personinterest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fc58-130">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fc58-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1fc58-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1fc58-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fc58-132">Request</span></span>

<span data-ttu-id="1fc58-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fc58-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fc58-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fc58-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personinterest_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/interests
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
# <a name="c"></a>[<span data-ttu-id="1fc58-135">C#</span><span class="sxs-lookup"><span data-stu-id="1fc58-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fc58-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fc58-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fc58-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fc58-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1fc58-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fc58-138">Response</span></span>

<span data-ttu-id="1fc58-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1fc58-139">The following is an example of the response.</span></span>

> <span data-ttu-id="1fc58-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fc58-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
  "description": "Create personInterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
