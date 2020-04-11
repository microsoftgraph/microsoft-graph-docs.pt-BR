---
title: Criar skillProficiency
description: Use esta API para criar um novo skillProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 17a0a1385423d4f8171bc9236afc1addf2f07d19
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228622"
---
# <a name="create-skillproficiency"></a><span data-ttu-id="f9c33-103">Criar skillProficiency</span><span class="sxs-lookup"><span data-stu-id="f9c33-103">Create skillProficiency</span></span>

<span data-ttu-id="f9c33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9c33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9c33-105">Use esta API para criar um novo objeto [skillProficiency](../resources/skillproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f9c33-105">Use this API to create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9c33-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9c33-106">Permissions</span></span>

<span data-ttu-id="f9c33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9c33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9c33-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9c33-109">Permission type</span></span>                        | <span data-ttu-id="f9c33-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9c33-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9c33-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9c33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9c33-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f9c33-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f9c33-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9c33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9c33-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f9c33-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f9c33-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9c33-115">Application</span></span>                            | <span data-ttu-id="f9c33-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c33-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f9c33-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9c33-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/skills
```

## <a name="request-headers"></a><span data-ttu-id="f9c33-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c33-118">Request headers</span></span>

| <span data-ttu-id="f9c33-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f9c33-119">Name</span></span>           | <span data-ttu-id="f9c33-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9c33-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="f9c33-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9c33-121">Authorization</span></span>  | <span data-ttu-id="f9c33-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9c33-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f9c33-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9c33-124">Content-Type</span></span>   | <span data-ttu-id="f9c33-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9c33-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9c33-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c33-127">Request body</span></span>

<span data-ttu-id="f9c33-128">No corpo da solicitação, forneça uma representação JSON do objeto [skillProficiency](../resources/skillproficiency.md) .</span><span class="sxs-lookup"><span data-stu-id="f9c33-128">In the request body, supply a JSON representation of [skillProficiency](../resources/skillproficiency.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f9c33-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9c33-129">Response</span></span>

<span data-ttu-id="f9c33-130">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [skillProficiency](../resources/skillproficiency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9c33-130">If successful, this method returns `201, Created` response code and a new [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9c33-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f9c33-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9c33-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9c33-132">Request</span></span>

<span data-ttu-id="f9c33-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9c33-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9c33-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9c33-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_skillproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/skills
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "displayName": "displayName-value",
  "proficiency": "proficiency-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f9c33-135">C#</span><span class="sxs-lookup"><span data-stu-id="f9c33-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-skillproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9c33-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9c33-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-skillproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9c33-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9c33-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-skillproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9c33-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9c33-138">Response</span></span>

<span data-ttu-id="f9c33-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9c33-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f9c33-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9c33-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "displayName": "displayName-value",
  "proficiency": "proficiency-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create skillProficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
