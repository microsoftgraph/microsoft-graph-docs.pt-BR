---
title: Criar personAnniversary
description: Use esta API para criar um novo personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d00734bf10467d8f76658fc3b6148f31f0201414
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455120"
---
# <a name="create-personanniversary"></a><span data-ttu-id="94e07-103">Criar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="94e07-103">Create personAnniversary</span></span>

<span data-ttu-id="94e07-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94e07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94e07-105">Use esta API para criar um novo objeto [personAnniversary](../resources/personanniversary.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="94e07-105">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94e07-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94e07-106">Permissions</span></span>

<span data-ttu-id="94e07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94e07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94e07-109">Permission type</span></span>                        | <span data-ttu-id="94e07-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94e07-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94e07-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94e07-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94e07-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="94e07-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="94e07-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94e07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94e07-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="94e07-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="94e07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94e07-115">Application</span></span>                            | <span data-ttu-id="94e07-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94e07-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="94e07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94e07-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries 
```

## <a name="request-headers"></a><span data-ttu-id="94e07-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94e07-118">Request headers</span></span>

| <span data-ttu-id="94e07-119">Nome</span><span class="sxs-lookup"><span data-stu-id="94e07-119">Name</span></span>      |<span data-ttu-id="94e07-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="94e07-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94e07-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="94e07-121">Authorization</span></span>  | <span data-ttu-id="94e07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94e07-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="94e07-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94e07-124">Content-Type</span></span>   | <span data-ttu-id="94e07-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94e07-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94e07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94e07-127">Request body</span></span>

<span data-ttu-id="94e07-128">No corpo da solicitação, forneça uma representação JSON do objeto [personAnniversary](../resources/personanniversary.md) .</span><span class="sxs-lookup"><span data-stu-id="94e07-128">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="94e07-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94e07-129">Response</span></span>

<span data-ttu-id="94e07-130">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [personAnniversary](../resources/personanniversary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94e07-130">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94e07-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="94e07-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94e07-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94e07-132">Request</span></span>

<span data-ttu-id="94e07-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94e07-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94e07-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94e07-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```
# <a name="c"></a>[<span data-ttu-id="94e07-135">C#</span><span class="sxs-lookup"><span data-stu-id="94e07-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personanniversary-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94e07-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94e07-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personanniversary-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94e07-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94e07-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personanniversary-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94e07-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="94e07-138">Response</span></span>

<span data-ttu-id="94e07-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94e07-139">The following is an example of the response.</span></span>

> <span data-ttu-id="94e07-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94e07-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personAnniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
