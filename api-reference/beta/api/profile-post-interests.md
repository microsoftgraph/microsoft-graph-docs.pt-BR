---
title: Criar personInterest
description: Criar um novo personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: ea7a3df0edcab0ed5b4f5cdf2307f01393772b13
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997812"
---
# <a name="create-personinterest"></a><span data-ttu-id="96b05-103">Criar personInterest</span><span class="sxs-lookup"><span data-stu-id="96b05-103">Create personInterest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96b05-104">Criar um novo [personInterest] (.. /resources/personinterest.md].</span><span class="sxs-lookup"><span data-stu-id="96b05-104">Create a new [personInterest](../resources/personinterest.md].</span></span>

## <a name="permissions"></a><span data-ttu-id="96b05-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="96b05-105">Permissions</span></span>

<span data-ttu-id="96b05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96b05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96b05-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96b05-108">Permission type</span></span>                        | <span data-ttu-id="96b05-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96b05-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96b05-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96b05-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="96b05-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96b05-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="96b05-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96b05-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96b05-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96b05-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="96b05-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96b05-114">Application</span></span>                            | <span data-ttu-id="96b05-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96b05-115">User.ReadWrite.All</span></span> |
## <a name="http-request"></a><span data-ttu-id="96b05-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96b05-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="96b05-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96b05-117">Request headers</span></span>

| <span data-ttu-id="96b05-118">Nome</span><span class="sxs-lookup"><span data-stu-id="96b05-118">Name</span></span>      |<span data-ttu-id="96b05-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="96b05-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96b05-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="96b05-120">Authorization</span></span>  | <span data-ttu-id="96b05-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96b05-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="96b05-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96b05-123">Content-Type</span></span>   | <span data-ttu-id="96b05-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96b05-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96b05-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96b05-126">Request body</span></span>

<span data-ttu-id="96b05-127">No corpo da solicitação, forneça uma representação JSON do objeto [personInterest](../resources/personinterest.md) .</span><span class="sxs-lookup"><span data-stu-id="96b05-127">In the request body, supply a JSON representation of [personInterest](../resources/personinterest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="96b05-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="96b05-128">Response</span></span>

<span data-ttu-id="96b05-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [personInterest](../resources/personinterest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96b05-129">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96b05-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="96b05-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96b05-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96b05-131">Request</span></span>

<span data-ttu-id="96b05-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96b05-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96b05-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="96b05-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="96b05-134">C#</span><span class="sxs-lookup"><span data-stu-id="96b05-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96b05-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96b05-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96b05-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96b05-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96b05-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="96b05-137">Response</span></span>

<span data-ttu-id="96b05-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96b05-138">The following is an example of the response.</span></span>

> <span data-ttu-id="96b05-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96b05-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
