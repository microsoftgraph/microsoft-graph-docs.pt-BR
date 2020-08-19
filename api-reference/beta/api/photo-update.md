---
title: Atualizar foto
description: Atualize as propriedades do objeto de foto.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: MSGraphDocsVteam
ms.openlocfilehash: d13411227dde53a582af5f3614fe5a6f4a3051cd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811623"
---
# <a name="update-photo"></a><span data-ttu-id="ee212-103">Atualizar foto</span><span class="sxs-lookup"><span data-stu-id="ee212-103">Update photo</span></span>

<span data-ttu-id="ee212-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee212-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee212-105">Atualize as propriedades do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="ee212-105">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee212-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee212-106">Permissions</span></span>
<span data-ttu-id="ee212-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee212-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee212-109">Permission type</span></span>      | <span data-ttu-id="ee212-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee212-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee212-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee212-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee212-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee212-112">Not supported.</span></span>    |
|<span data-ttu-id="ee212-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee212-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee212-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee212-114">Not supported.</span></span>    |
|<span data-ttu-id="ee212-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee212-115">Application</span></span> | <span data-ttu-id="ee212-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee212-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee212-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee212-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="ee212-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee212-118">Request headers</span></span>
| <span data-ttu-id="ee212-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ee212-119">Name</span></span>       | <span data-ttu-id="ee212-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee212-120">Type</span></span> | <span data-ttu-id="ee212-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee212-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ee212-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee212-122">Authorization</span></span>  | <span data-ttu-id="ee212-123">string</span><span class="sxs-lookup"><span data-stu-id="ee212-123">string</span></span>  | <span data-ttu-id="ee212-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee212-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee212-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee212-126">Request body</span></span>
<span data-ttu-id="ee212-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ee212-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ee212-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee212-130">Property</span></span>     | <span data-ttu-id="ee212-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee212-131">Type</span></span>   |<span data-ttu-id="ee212-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee212-132">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="ee212-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee212-133">Response</span></span>

<span data-ttu-id="ee212-134">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [photo](../resources/photo.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee212-134">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee212-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee212-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee212-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee212-136">Request</span></span>
<span data-ttu-id="ee212-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee212-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee212-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee212-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ee212-139">C#</span><span class="sxs-lookup"><span data-stu-id="ee212-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee212-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee212-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee212-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee212-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ee212-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee212-142">Response</span></span>
<span data-ttu-id="ee212-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee212-143">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
