---
title: Atualizar a categoria do Outlook
description: 'Atualize a propriedade gravável, **color**, do objeto outlookCategory especificado. Não é possível modificar a propriedade **DisplayName** '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7c6e101b524c5563419169513a2fdc715dabee1a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349901"
---
# <a name="update-outlook-category"></a><span data-ttu-id="94454-104">Atualizar a categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="94454-104">Update Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94454-105">Atualize a propriedade gravável, **color**, do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="94454-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="94454-106">Não é possível modificar a propriedade **displayName** depois de criar a categoria.</span><span class="sxs-lookup"><span data-stu-id="94454-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="94454-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94454-107">Permissions</span></span>
<span data-ttu-id="94454-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94454-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94454-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94454-110">Permission type</span></span>      | <span data-ttu-id="94454-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94454-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94454-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94454-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94454-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94454-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="94454-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94454-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94454-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94454-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="94454-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94454-116">Application</span></span> | <span data-ttu-id="94454-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94454-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94454-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94454-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94454-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94454-119">Request headers</span></span>
| <span data-ttu-id="94454-120">Nome</span><span class="sxs-lookup"><span data-stu-id="94454-120">Name</span></span>      |<span data-ttu-id="94454-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94454-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94454-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94454-122">Authorization</span></span>  | <span data-ttu-id="94454-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94454-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94454-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94454-125">Request body</span></span>
<span data-ttu-id="94454-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="94454-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94454-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94454-129">Property</span></span>     | <span data-ttu-id="94454-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="94454-130">Type</span></span>   |<span data-ttu-id="94454-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="94454-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94454-132">color</span><span class="sxs-lookup"><span data-stu-id="94454-132">color</span></span>|<span data-ttu-id="94454-133">String</span><span class="sxs-lookup"><span data-stu-id="94454-133">String</span></span>|<span data-ttu-id="94454-134">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="94454-134">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="94454-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="94454-135">Response</span></span>

<span data-ttu-id="94454-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94454-136">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94454-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94454-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94454-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94454-138">Request</span></span>
<span data-ttu-id="94454-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94454-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94454-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="94454-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94454-141">C#</span><span class="sxs-lookup"><span data-stu-id="94454-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94454-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94454-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94454-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="94454-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="94454-144">Java</span><span class="sxs-lookup"><span data-stu-id="94454-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94454-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="94454-145">Response</span></span>
<span data-ttu-id="94454-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94454-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
