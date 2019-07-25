---
title: Atualizar administrativeunit
description: Atualiza as propriedades de um objeto administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5953e67b86503c0736d9bbab551d7bd393b4c944
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855551"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="f50c6-103">Atualizar administrativeunit</span><span class="sxs-lookup"><span data-stu-id="f50c6-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f50c6-104">Atualiza as propriedades de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="f50c6-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f50c6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f50c6-105">Permissions</span></span>
<span data-ttu-id="f50c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f50c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f50c6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f50c6-108">Permission type</span></span>      | <span data-ttu-id="f50c6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f50c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f50c6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f50c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f50c6-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f50c6-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f50c6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f50c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f50c6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f50c6-113">Not supported.</span></span>    |
|<span data-ttu-id="f50c6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f50c6-114">Application</span></span> | <span data-ttu-id="f50c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f50c6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f50c6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f50c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f50c6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f50c6-117">Request headers</span></span>

| <span data-ttu-id="f50c6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f50c6-118">Name</span></span>      |<span data-ttu-id="f50c6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f50c6-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f50c6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f50c6-120">Authorization</span></span>  | <span data-ttu-id="f50c6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f50c6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f50c6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f50c6-123">Request body</span></span>

<span data-ttu-id="f50c6-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f50c6-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f50c6-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f50c6-127">Property</span></span>   | <span data-ttu-id="f50c6-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f50c6-128">Type</span></span> |<span data-ttu-id="f50c6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f50c6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f50c6-130">description</span><span class="sxs-lookup"><span data-stu-id="f50c6-130">description</span></span>|<span data-ttu-id="f50c6-131">string</span><span class="sxs-lookup"><span data-stu-id="f50c6-131">string</span></span>|<span data-ttu-id="f50c6-132">Descrição da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="f50c6-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="f50c6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f50c6-133">displayName</span></span>|<span data-ttu-id="f50c6-134">string</span><span class="sxs-lookup"><span data-stu-id="f50c6-134">string</span></span>|<span data-ttu-id="f50c6-135">Nome de exibição para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="f50c6-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="f50c6-136">visibilidade</span><span class="sxs-lookup"><span data-stu-id="f50c6-136">visibility</span></span>|<span data-ttu-id="f50c6-137">string</span><span class="sxs-lookup"><span data-stu-id="f50c6-137">string</span></span>|<span data-ttu-id="f50c6-138">Visibilidade para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="f50c6-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="f50c6-139">Se não for definido, o padrão será "Public".</span><span class="sxs-lookup"><span data-stu-id="f50c6-139">If not set then the default is "public".</span></span> <span data-ttu-id="f50c6-140">Pode ser definido como "HiddenMembership", que oculta a associação de não membros.</span><span class="sxs-lookup"><span data-stu-id="f50c6-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="f50c6-141">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode `PATCH` usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância existente do **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="f50c6-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="f50c6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f50c6-142">Response</span></span>

<span data-ttu-id="f50c6-143">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f50c6-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f50c6-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f50c6-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f50c6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f50c6-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f50c6-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f50c6-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f50c6-147">C#</span><span class="sxs-lookup"><span data-stu-id="f50c6-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f50c6-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="f50c6-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f50c6-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f50c6-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f50c6-150">Java</span><span class="sxs-lookup"><span data-stu-id="f50c6-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f50c6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f50c6-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="f50c6-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="f50c6-152">See also</span></span>

- [<span data-ttu-id="f50c6-153">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="f50c6-153">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f50c6-154">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="f50c6-154">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
