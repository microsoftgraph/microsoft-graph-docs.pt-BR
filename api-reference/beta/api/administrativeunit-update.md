---
title: Atualizar administrativeunit
description: Atualize as propriedades de um objeto administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c02cb7944672c64f20768ed0edc0ca254564fc62
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786605"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="472f4-103">Atualizar administrativeunit</span><span class="sxs-lookup"><span data-stu-id="472f4-103">Update administrativeunit</span></span>

<span data-ttu-id="472f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="472f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="472f4-105">Atualize as propriedades de [um objeto administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="472f4-105">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="472f4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="472f4-106">Permissions</span></span>
<span data-ttu-id="472f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="472f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="472f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="472f4-109">Permission type</span></span>      | <span data-ttu-id="472f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="472f4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="472f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="472f4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="472f4-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="472f4-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="472f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="472f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="472f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="472f4-114">Not supported.</span></span>    |
|<span data-ttu-id="472f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="472f4-115">Application</span></span> | <span data-ttu-id="472f4-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="472f4-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="472f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="472f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="472f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="472f4-118">Request headers</span></span>

| <span data-ttu-id="472f4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="472f4-119">Name</span></span>      |<span data-ttu-id="472f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="472f4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="472f4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="472f4-121">Authorization</span></span>  | <span data-ttu-id="472f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="472f4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="472f4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="472f4-124">Request body</span></span>

<span data-ttu-id="472f4-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="472f4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="472f4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="472f4-128">Property</span></span>   | <span data-ttu-id="472f4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="472f4-129">Type</span></span> |<span data-ttu-id="472f4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="472f4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="472f4-131">description</span><span class="sxs-lookup"><span data-stu-id="472f4-131">description</span></span>|<span data-ttu-id="472f4-132">string</span><span class="sxs-lookup"><span data-stu-id="472f4-132">string</span></span>|<span data-ttu-id="472f4-133">Descrição da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="472f4-133">Description for the administrative unit.</span></span>|
|<span data-ttu-id="472f4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="472f4-134">displayName</span></span>|<span data-ttu-id="472f4-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472f4-135">string</span></span>|<span data-ttu-id="472f4-136">Nome de exibição da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="472f4-136">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="472f4-137">visibilidade</span><span class="sxs-lookup"><span data-stu-id="472f4-137">visibility</span></span>|<span data-ttu-id="472f4-138">string</span><span class="sxs-lookup"><span data-stu-id="472f4-138">string</span></span>|<span data-ttu-id="472f4-139">Visibilidade da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="472f4-139">Visibility for the administrative unit.</span></span> <span data-ttu-id="472f4-140">Se não for definido, o padrão será "público".</span><span class="sxs-lookup"><span data-stu-id="472f4-140">If not set then the default is "public".</span></span> <span data-ttu-id="472f4-141">Pode ser definido como "HiddenMembership", que oculta a associação de não membros.</span><span class="sxs-lookup"><span data-stu-id="472f4-141">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="472f4-142">Como o **recurso administrativeUnit** dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância `PATCH` **administrativeUnit** existente.</span><span class="sxs-lookup"><span data-stu-id="472f4-142">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="472f4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="472f4-143">Response</span></span>

<span data-ttu-id="472f4-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="472f4-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="472f4-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="472f4-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="472f4-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="472f4-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="472f4-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="472f4-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="472f4-148">C#</span><span class="sxs-lookup"><span data-stu-id="472f4-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="472f4-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="472f4-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="472f4-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="472f4-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="472f4-151">Java</span><span class="sxs-lookup"><span data-stu-id="472f4-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="472f4-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="472f4-152">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="472f4-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="472f4-153">See also</span></span>

- [<span data-ttu-id="472f4-154">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="472f4-154">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="472f4-155">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="472f4-155">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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


