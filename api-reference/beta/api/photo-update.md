---
title: Atualizar foto
description: Atualize as propriedades do objeto de foto.
localization_priority: Normal
ms.openlocfilehash: 0d12b83f7c9436cce14a27ed5f27741b4ac92da3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876900"
---
# <a name="update-photo"></a><span data-ttu-id="8cdf5-103">Atualizar foto</span><span class="sxs-lookup"><span data-stu-id="8cdf5-103">Update photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cdf5-104">Atualize as propriedades do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8cdf5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cdf5-105">Permissions</span></span>
<span data-ttu-id="8cdf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cdf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cdf5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cdf5-108">Permission type</span></span>      | <span data-ttu-id="8cdf5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cdf5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cdf5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cdf5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8cdf5-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-111">Not supported.</span></span>    |
|<span data-ttu-id="8cdf5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cdf5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cdf5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-113">Not supported.</span></span>    |
|<span data-ttu-id="8cdf5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cdf5-114">Application</span></span> | <span data-ttu-id="8cdf5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cdf5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cdf5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="8cdf5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cdf5-117">Request headers</span></span>
| <span data-ttu-id="8cdf5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8cdf5-118">Name</span></span>       | <span data-ttu-id="8cdf5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cdf5-119">Type</span></span> | <span data-ttu-id="8cdf5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cdf5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8cdf5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cdf5-121">Authorization</span></span>  | <span data-ttu-id="8cdf5-122">string</span><span class="sxs-lookup"><span data-stu-id="8cdf5-122">string</span></span>  | <span data-ttu-id="8cdf5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cdf5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cdf5-125">Request body</span></span>
<span data-ttu-id="8cdf5-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8cdf5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cdf5-129">Property</span></span>     | <span data-ttu-id="8cdf5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cdf5-130">Type</span></span>   |<span data-ttu-id="8cdf5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cdf5-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="8cdf5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cdf5-132">Response</span></span>

<span data-ttu-id="8cdf5-133">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [photo](../resources/photo.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cdf5-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cdf5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cdf5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cdf5-135">Request</span></span>
<span data-ttu-id="8cdf5-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8cdf5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cdf5-137">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8cdf5-138">C#</span><span class="sxs-lookup"><span data-stu-id="8cdf5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cdf5-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="8cdf5-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8cdf5-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8cdf5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8cdf5-141">Java</span><span class="sxs-lookup"><span data-stu-id="8cdf5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8cdf5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cdf5-142">Response</span></span>
<span data-ttu-id="8cdf5-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cdf5-143">Here is an example of the response.</span></span>
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
