---
title: Atualizar administrativeunit
description: Atualiza as propriedades de um objeto administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9df55c0292c51b509ba9d3d79eb1e41b27065cfb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439851"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="a5b52-103">Atualizar administrativeunit</span><span class="sxs-lookup"><span data-stu-id="a5b52-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5b52-104">Atualiza as propriedades de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="a5b52-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a5b52-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5b52-105">Permissions</span></span>
<span data-ttu-id="a5b52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5b52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5b52-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5b52-108">Permission type</span></span>      | <span data-ttu-id="a5b52-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5b52-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5b52-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5b52-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5b52-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5b52-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5b52-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5b52-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5b52-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5b52-113">Not supported.</span></span>    |
|<span data-ttu-id="a5b52-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5b52-114">Application</span></span> | <span data-ttu-id="a5b52-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5b52-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5b52-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5b52-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5b52-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b52-117">Request headers</span></span>

| <span data-ttu-id="a5b52-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a5b52-118">Name</span></span>      |<span data-ttu-id="a5b52-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5b52-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5b52-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5b52-120">Authorization</span></span>  | <span data-ttu-id="a5b52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5b52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5b52-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b52-123">Request body</span></span>

<span data-ttu-id="a5b52-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a5b52-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a5b52-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5b52-127">Property</span></span>   | <span data-ttu-id="a5b52-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5b52-128">Type</span></span> |<span data-ttu-id="a5b52-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5b52-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5b52-130">description</span><span class="sxs-lookup"><span data-stu-id="a5b52-130">description</span></span>|<span data-ttu-id="a5b52-131">string</span><span class="sxs-lookup"><span data-stu-id="a5b52-131">string</span></span>|<span data-ttu-id="a5b52-132">Descrição da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="a5b52-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="a5b52-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a5b52-133">displayName</span></span>|<span data-ttu-id="a5b52-134">string</span><span class="sxs-lookup"><span data-stu-id="a5b52-134">string</span></span>|<span data-ttu-id="a5b52-135">Nome de exibição para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="a5b52-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="a5b52-136">visibilidade</span><span class="sxs-lookup"><span data-stu-id="a5b52-136">visibility</span></span>|<span data-ttu-id="a5b52-137">string</span><span class="sxs-lookup"><span data-stu-id="a5b52-137">string</span></span>|<span data-ttu-id="a5b52-138">Visibilidade para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="a5b52-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="a5b52-139">Se não for definido, o padrão será "Public".</span><span class="sxs-lookup"><span data-stu-id="a5b52-139">If not set then the default is "public".</span></span> <span data-ttu-id="a5b52-140">Pode ser definido como "HiddenMembership", que oculta a associação de não membros.</span><span class="sxs-lookup"><span data-stu-id="a5b52-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="a5b52-141">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode `PATCH` usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância existente do **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="a5b52-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="a5b52-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5b52-142">Response</span></span>

<span data-ttu-id="a5b52-143">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5b52-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5b52-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5b52-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5b52-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5b52-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a5b52-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5b52-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5b52-147">C#</span><span class="sxs-lookup"><span data-stu-id="a5b52-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5b52-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5b52-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5b52-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a5b52-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5b52-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5b52-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="a5b52-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="a5b52-151">See also</span></span>

- [<span data-ttu-id="a5b52-152">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="a5b52-152">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a5b52-153">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="a5b52-153">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
