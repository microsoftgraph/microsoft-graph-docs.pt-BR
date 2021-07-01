---
title: Atualizar administrativeunit
description: Atualize as propriedades de um objeto administrativeUnit.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0921bc6366d34278d23701d11ddb21bf0793d219
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208208"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="ecff8-103">Atualizar administrativeunit</span><span class="sxs-lookup"><span data-stu-id="ecff8-103">Update administrativeunit</span></span>

<span data-ttu-id="ecff8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecff8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecff8-105">Atualize as propriedades de [um objeto administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="ecff8-105">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ecff8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecff8-106">Permissions</span></span>
<span data-ttu-id="ecff8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecff8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ecff8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecff8-109">Permission type</span></span>      | <span data-ttu-id="ecff8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecff8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecff8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecff8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ecff8-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ecff8-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ecff8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecff8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecff8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecff8-114">Not supported.</span></span>    |
|<span data-ttu-id="ecff8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecff8-115">Application</span></span> | <span data-ttu-id="ecff8-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecff8-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecff8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecff8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /directory/administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ecff8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecff8-118">Request headers</span></span>

| <span data-ttu-id="ecff8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ecff8-119">Name</span></span>      |<span data-ttu-id="ecff8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecff8-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ecff8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecff8-121">Authorization</span></span>  | <span data-ttu-id="ecff8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecff8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ecff8-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ecff8-124">Content-type</span></span> | <span data-ttu-id="ecff8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecff8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecff8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecff8-127">Request body</span></span>

<span data-ttu-id="ecff8-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ecff8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ecff8-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecff8-131">Property</span></span>   | <span data-ttu-id="ecff8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecff8-132">Type</span></span> |<span data-ttu-id="ecff8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecff8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecff8-134">description</span><span class="sxs-lookup"><span data-stu-id="ecff8-134">description</span></span>|<span data-ttu-id="ecff8-135">string</span><span class="sxs-lookup"><span data-stu-id="ecff8-135">string</span></span>|<span data-ttu-id="ecff8-136">Descrição da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="ecff8-136">Description for the administrative unit.</span></span>|
|<span data-ttu-id="ecff8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ecff8-137">displayName</span></span>|<span data-ttu-id="ecff8-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecff8-138">string</span></span>|<span data-ttu-id="ecff8-139">Nome de exibição da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="ecff8-139">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="ecff8-140">visibilidade</span><span class="sxs-lookup"><span data-stu-id="ecff8-140">visibility</span></span>|<span data-ttu-id="ecff8-141">string</span><span class="sxs-lookup"><span data-stu-id="ecff8-141">string</span></span>|<span data-ttu-id="ecff8-142">Visibilidade da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="ecff8-142">Visibility for the administrative unit.</span></span> <span data-ttu-id="ecff8-143">Se não for definido, o padrão será "público".</span><span class="sxs-lookup"><span data-stu-id="ecff8-143">If not set then the default is "public".</span></span> <span data-ttu-id="ecff8-144">Pode ser definido como "HiddenMembership", que oculta a associação de não membros.</span><span class="sxs-lookup"><span data-stu-id="ecff8-144">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="ecff8-145">Como o **recurso administrativeUnit** dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância `PATCH` **administrativeUnit** existente.</span><span class="sxs-lookup"><span data-stu-id="ecff8-145">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="ecff8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecff8-146">Response</span></span>

<span data-ttu-id="ecff8-147">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ecff8-147">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ecff8-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecff8-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ecff8-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecff8-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ecff8-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecff8-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ecff8-151">C#</span><span class="sxs-lookup"><span data-stu-id="ecff8-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecff8-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecff8-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecff8-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecff8-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecff8-154">Java</span><span class="sxs-lookup"><span data-stu-id="ecff8-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


##### <a name="response"></a><span data-ttu-id="ecff8-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecff8-155">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="ecff8-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="ecff8-156">See also</span></span>

- [<span data-ttu-id="ecff8-157">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="ecff8-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ecff8-158">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="ecff8-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
