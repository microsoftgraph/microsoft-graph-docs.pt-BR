---
title: Atualizar foto
description: Atualize as propriedades do objeto de foto.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 41ce52fb4de9348b8bec9ea2e99848ee230cb268
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511016"
---
# <a name="update-photo"></a><span data-ttu-id="8e1bc-103">Atualizar foto</span><span class="sxs-lookup"><span data-stu-id="8e1bc-103">Update photo</span></span>

<span data-ttu-id="8e1bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e1bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e1bc-105">Atualize as propriedades do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-105">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8e1bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e1bc-106">Permissions</span></span>
<span data-ttu-id="8e1bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e1bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e1bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e1bc-109">Permission type</span></span>      | <span data-ttu-id="8e1bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e1bc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e1bc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e1bc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8e1bc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-112">Not supported.</span></span>    |
|<span data-ttu-id="8e1bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e1bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e1bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-114">Not supported.</span></span>    |
|<span data-ttu-id="8e1bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e1bc-115">Application</span></span> | <span data-ttu-id="8e1bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e1bc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e1bc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="8e1bc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e1bc-118">Request headers</span></span>
| <span data-ttu-id="8e1bc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8e1bc-119">Name</span></span>       | <span data-ttu-id="8e1bc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e1bc-120">Type</span></span> | <span data-ttu-id="8e1bc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e1bc-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8e1bc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e1bc-122">Authorization</span></span>  | <span data-ttu-id="8e1bc-123">string</span><span class="sxs-lookup"><span data-stu-id="8e1bc-123">string</span></span>  | <span data-ttu-id="8e1bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e1bc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e1bc-126">Request body</span></span>
<span data-ttu-id="8e1bc-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e1bc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e1bc-130">Property</span></span>     | <span data-ttu-id="8e1bc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e1bc-131">Type</span></span>   |<span data-ttu-id="8e1bc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e1bc-132">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="8e1bc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e1bc-133">Response</span></span>

<span data-ttu-id="8e1bc-134">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [photo](../resources/photo.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-134">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e1bc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e1bc-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e1bc-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e1bc-136">Request</span></span>
<span data-ttu-id="8e1bc-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e1bc-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e1bc-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
# <a name="c"></a>[<span data-ttu-id="8e1bc-139">C#</span><span class="sxs-lookup"><span data-stu-id="8e1bc-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e1bc-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e1bc-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e1bc-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e1bc-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e1bc-142">Java</span><span class="sxs-lookup"><span data-stu-id="8e1bc-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8e1bc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e1bc-143">Response</span></span>
<span data-ttu-id="8e1bc-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e1bc-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
