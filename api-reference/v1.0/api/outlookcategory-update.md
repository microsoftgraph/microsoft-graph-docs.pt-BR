---
title: Atualizar a categoria do Outlook
description: 'Atualize a propriedade gravável, **color**, do objeto outlookCategory especificado. Não é possível modificar a propriedade **DisplayName** '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 623653f292ddc67c491537e7e60ceeaa900dd655
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511135"
---
# <a name="update-outlook-category"></a><span data-ttu-id="21355-104">Atualizar a categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="21355-104">Update Outlook category</span></span>

<span data-ttu-id="21355-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21355-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="21355-106">Atualize a propriedade gravável, **color**, do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="21355-106">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="21355-107">Não é possível modificar a propriedade **displayName** depois de criar a categoria.</span><span class="sxs-lookup"><span data-stu-id="21355-107">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="21355-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="21355-108">Permissions</span></span>
<span data-ttu-id="21355-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21355-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21355-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21355-111">Permission type</span></span>      | <span data-ttu-id="21355-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21355-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21355-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21355-113">Delegated (work or school account)</span></span> | <span data-ttu-id="21355-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21355-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="21355-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21355-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21355-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21355-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="21355-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21355-117">Application</span></span> | <span data-ttu-id="21355-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21355-118">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="21355-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21355-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21355-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21355-120">Request headers</span></span>
| <span data-ttu-id="21355-121">Nome</span><span class="sxs-lookup"><span data-stu-id="21355-121">Name</span></span>      |<span data-ttu-id="21355-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="21355-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21355-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21355-123">Authorization</span></span>  | <span data-ttu-id="21355-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21355-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21355-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21355-126">Request body</span></span>
<span data-ttu-id="21355-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="21355-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="21355-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21355-130">Property</span></span>     | <span data-ttu-id="21355-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="21355-131">Type</span></span>   |<span data-ttu-id="21355-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="21355-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21355-133">color</span><span class="sxs-lookup"><span data-stu-id="21355-133">color</span></span>|<span data-ttu-id="21355-134">String</span><span class="sxs-lookup"><span data-stu-id="21355-134">String</span></span>|<span data-ttu-id="21355-135">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="21355-135">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="21355-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="21355-136">Response</span></span>

<span data-ttu-id="21355-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21355-137">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21355-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21355-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21355-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21355-139">Request</span></span>
<span data-ttu-id="21355-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21355-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21355-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="21355-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
# <a name="c"></a>[<span data-ttu-id="21355-142">C#</span><span class="sxs-lookup"><span data-stu-id="21355-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21355-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21355-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21355-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21355-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21355-145">Java</span><span class="sxs-lookup"><span data-stu-id="21355-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="21355-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="21355-146">Response</span></span>
<span data-ttu-id="21355-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21355-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
