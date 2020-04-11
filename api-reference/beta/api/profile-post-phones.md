---
title: Criar um número de telefone
description: Use esta API para criar um novo Multiphone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 54fb9ff1453573fbf8c2904d581f54790093dfa6
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229315"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="6723c-103">Criar itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="6723c-103">Create itemPhoneNumber</span></span>

<span data-ttu-id="6723c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6723c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6723c-105">Use esta API para criar um novo objeto [MyPhone](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="6723c-105">Use this API to create a new [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6723c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6723c-106">Permissions</span></span>

<span data-ttu-id="6723c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6723c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6723c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6723c-109">Permission type</span></span>                        | <span data-ttu-id="6723c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6723c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6723c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6723c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6723c-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6723c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6723c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6723c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6723c-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6723c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6723c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6723c-115">Application</span></span>                            | <span data-ttu-id="6723c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6723c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="6723c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6723c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="6723c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6723c-118">Request headers</span></span>

| <span data-ttu-id="6723c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6723c-119">Name</span></span>           | <span data-ttu-id="6723c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6723c-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="6723c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6723c-121">Authorization</span></span>  | <span data-ttu-id="6723c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6723c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6723c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6723c-124">Content-Type</span></span>   | <span data-ttu-id="6723c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6723c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6723c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6723c-127">Request body</span></span>

<span data-ttu-id="6723c-128">No corpo da solicitação, forneça uma representação JSON do objeto [MyPhone](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="6723c-128">In the request body, supply a JSON representation of [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6723c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6723c-129">Response</span></span>

<span data-ttu-id="6723c-130">Se bem-sucedido, este método retorna `201, Created` o código de resposta e um novo objeto [MyPhone](../resources/itemphone.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6723c-130">If successful, this method returns `201, Created` response code and a new [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6723c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6723c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6723c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6723c-132">Request</span></span>

<span data-ttu-id="6723c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6723c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6723c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6723c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemphone_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/phones
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6723c-135">C#</span><span class="sxs-lookup"><span data-stu-id="6723c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6723c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6723c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6723c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6723c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6723c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6723c-138">Response</span></span>

<span data-ttu-id="6723c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6723c-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6723c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6723c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
