---
title: Criar personInterest
description: Criar um novo personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: 390526786ae6761259ae6a83cec987dbcf74d6db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455099"
---
# <a name="create-personinterest"></a><span data-ttu-id="e666b-103">Criar personInterest</span><span class="sxs-lookup"><span data-stu-id="e666b-103">Create personInterest</span></span>

<span data-ttu-id="e666b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e666b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e666b-105">Criar um novo [personInterest] (.. /resources/personinterest.md].</span><span class="sxs-lookup"><span data-stu-id="e666b-105">Create a new [personInterest](../resources/personinterest.md].</span></span>

## <a name="permissions"></a><span data-ttu-id="e666b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e666b-106">Permissions</span></span>

<span data-ttu-id="e666b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e666b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e666b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e666b-109">Permission type</span></span>                        | <span data-ttu-id="e666b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e666b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e666b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e666b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e666b-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e666b-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e666b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e666b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e666b-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e666b-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e666b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e666b-115">Application</span></span>                            | <span data-ttu-id="e666b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e666b-116">User.ReadWrite.All</span></span> |
## <a name="http-request"></a><span data-ttu-id="e666b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e666b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="e666b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e666b-118">Request headers</span></span>

| <span data-ttu-id="e666b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e666b-119">Name</span></span>      |<span data-ttu-id="e666b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e666b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e666b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e666b-121">Authorization</span></span>  | <span data-ttu-id="e666b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e666b-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e666b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e666b-124">Content-Type</span></span>   | <span data-ttu-id="e666b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e666b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e666b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e666b-127">Request body</span></span>

<span data-ttu-id="e666b-128">No corpo da solicitação, forneça uma representação JSON do objeto [personInterest](../resources/personinterest.md) .</span><span class="sxs-lookup"><span data-stu-id="e666b-128">In the request body, supply a JSON representation of [personInterest](../resources/personinterest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e666b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e666b-129">Response</span></span>

<span data-ttu-id="e666b-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [personInterest](../resources/personinterest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e666b-130">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e666b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e666b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e666b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e666b-132">Request</span></span>

<span data-ttu-id="e666b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e666b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e666b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e666b-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e666b-135">C#</span><span class="sxs-lookup"><span data-stu-id="e666b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e666b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e666b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e666b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e666b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e666b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e666b-138">Response</span></span>

<span data-ttu-id="e666b-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e666b-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e666b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e666b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
