---
title: Criar um número de telefone
description: Use esta API para criar um novo Multiphone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 07d19b6c773f1b92a295f0c1e3471942dda45696
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996521"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="e2a7d-103">Criar itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e2a7d-103">Create itemPhoneNumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2a7d-104">Use esta API para criar um novo objeto [MyPhone](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="e2a7d-104">Use this API to create a new [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2a7d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2a7d-105">Permissions</span></span>

<span data-ttu-id="e2a7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2a7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2a7d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2a7d-108">Permission type</span></span>                        | <span data-ttu-id="e2a7d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2a7d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2a7d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2a7d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2a7d-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e2a7d-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e2a7d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2a7d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2a7d-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e2a7d-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e2a7d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2a7d-114">Application</span></span>                            | <span data-ttu-id="e2a7d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2a7d-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2a7d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a7d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="e2a7d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a7d-117">Request headers</span></span>

| <span data-ttu-id="e2a7d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e2a7d-118">Name</span></span>      |<span data-ttu-id="e2a7d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2a7d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2a7d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2a7d-120">Authorization</span></span>  | <span data-ttu-id="e2a7d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2a7d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e2a7d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2a7d-123">Content-Type</span></span>   | <span data-ttu-id="e2a7d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2a7d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2a7d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a7d-126">Request body</span></span>

<span data-ttu-id="e2a7d-127">No corpo da solicitação, forneça uma representação JSON do objeto [MyPhone](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="e2a7d-127">In the request body, supply a JSON representation of [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2a7d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a7d-128">Response</span></span>

<span data-ttu-id="e2a7d-129">Se bem-sucedido, este método retorna `201, Created` o código de resposta e um novo objeto [MyPhone](../resources/itemphone.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a7d-129">If successful, this method returns `201, Created` response code and a new [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2a7d-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e2a7d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2a7d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a7d-131">Request</span></span>

<span data-ttu-id="e2a7d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2a7d-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2a7d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a7d-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2a7d-134">C#</span><span class="sxs-lookup"><span data-stu-id="e2a7d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2a7d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2a7d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2a7d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2a7d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2a7d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a7d-137">Response</span></span>

<span data-ttu-id="e2a7d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a7d-138">The following is an example of the response.</span></span>

> <span data-ttu-id="e2a7d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2a7d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
