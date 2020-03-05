---
title: Criar PersonName
description: Use esta API para criar um novo PersonName no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: dd9b66db16f3c9146b47e917d9417ac7bb7e7adb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455082"
---
# <a name="create-personname"></a><span data-ttu-id="6dff0-103">Criar PersonName</span><span class="sxs-lookup"><span data-stu-id="6dff0-103">Create personName</span></span>

<span data-ttu-id="6dff0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6dff0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dff0-105">Use esta API para criar um novo objeto [PersonName](../resources/personname.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6dff0-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6dff0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6dff0-106">Permissions</span></span>

<span data-ttu-id="6dff0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6dff0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dff0-109">Permission type</span></span>                        | <span data-ttu-id="6dff0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dff0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="6dff0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dff0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6dff0-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6dff0-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6dff0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dff0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dff0-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6dff0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6dff0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dff0-115">Application</span></span>                            | <span data-ttu-id="6dff0-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6dff0-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dff0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dff0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="6dff0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dff0-118">Request headers</span></span>

| <span data-ttu-id="6dff0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6dff0-119">Name</span></span>           |<span data-ttu-id="6dff0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dff0-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="6dff0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dff0-121">Authorization</span></span>  | <span data-ttu-id="6dff0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dff0-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6dff0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6dff0-124">Content-Type</span></span>   | <span data-ttu-id="6dff0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dff0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dff0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dff0-127">Request body</span></span>

<span data-ttu-id="6dff0-128">No corpo da solicitação, forneça uma representação JSON do objeto [PersonName](../resources/personname.md) .</span><span class="sxs-lookup"><span data-stu-id="6dff0-128">In the request body, supply a JSON representation of [personName](../resources/personname.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6dff0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dff0-129">Response</span></span>

<span data-ttu-id="6dff0-130">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [PersonName](../resources/personname.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dff0-130">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6dff0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6dff0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dff0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dff0-132">Request</span></span>

<span data-ttu-id="6dff0-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dff0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6dff0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dff0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6dff0-135">C#</span><span class="sxs-lookup"><span data-stu-id="6dff0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6dff0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dff0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6dff0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dff0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6dff0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dff0-138">Response</span></span>

<span data-ttu-id="6dff0-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6dff0-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6dff0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dff0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
