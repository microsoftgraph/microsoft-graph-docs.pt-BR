---
title: Atualizar administrativeunit
description: Atualiza as propriedades de um objeto administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f3c57f8784bf642df7944bc6295ebd4fadc0ba43
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459278"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="0d3d3-103">Atualizar administrativeunit</span><span class="sxs-lookup"><span data-stu-id="0d3d3-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d3d3-104">Atualiza as propriedades de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="0d3d3-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d3d3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d3d3-105">Permissions</span></span>
<span data-ttu-id="0d3d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d3d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0d3d3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d3d3-108">Permission type</span></span>      | <span data-ttu-id="0d3d3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d3d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d3d3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d3d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d3d3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d3d3-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d3d3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d3d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d3d3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-113">Not supported.</span></span>    |
|<span data-ttu-id="0d3d3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d3d3-114">Application</span></span> | <span data-ttu-id="0d3d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d3d3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d3d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d3d3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d3d3-117">Request headers</span></span>

| <span data-ttu-id="0d3d3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0d3d3-118">Name</span></span>      |<span data-ttu-id="0d3d3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d3d3-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d3d3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d3d3-120">Authorization</span></span>  | <span data-ttu-id="0d3d3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d3d3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d3d3-123">Request body</span></span>

<span data-ttu-id="0d3d3-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d3d3-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d3d3-127">Property</span></span>   | <span data-ttu-id="0d3d3-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d3d3-128">Type</span></span> |<span data-ttu-id="0d3d3-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d3d3-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d3d3-130">description</span><span class="sxs-lookup"><span data-stu-id="0d3d3-130">description</span></span>|<span data-ttu-id="0d3d3-131">string</span><span class="sxs-lookup"><span data-stu-id="0d3d3-131">string</span></span>|<span data-ttu-id="0d3d3-132">Descrição da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="0d3d3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0d3d3-133">displayName</span></span>|<span data-ttu-id="0d3d3-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d3d3-134">string</span></span>|<span data-ttu-id="0d3d3-135">Nome de exibição para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="0d3d3-136">visibility</span><span class="sxs-lookup"><span data-stu-id="0d3d3-136">visibility</span></span>|<span data-ttu-id="0d3d3-137">string</span><span class="sxs-lookup"><span data-stu-id="0d3d3-137">string</span></span>|<span data-ttu-id="0d3d3-138">Visibilidade para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="0d3d3-139">Se não for definido, o padrão será "Public".</span><span class="sxs-lookup"><span data-stu-id="0d3d3-139">If not set then the default is "public".</span></span> <span data-ttu-id="0d3d3-140">Pode ser definido como "HiddenMembership", que oculta a associação de não membros.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="0d3d3-141">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode `PATCH` usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância existente do **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="0d3d3-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="0d3d3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d3d3-142">Response</span></span>

<span data-ttu-id="0d3d3-143">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d3d3-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d3d3-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d3d3-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0d3d3-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d3d3-145">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="0d3d3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d3d3-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="0d3d3-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="0d3d3-147">See also</span></span>

- [<span data-ttu-id="0d3d3-148">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="0d3d3-148">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0d3d3-149">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="0d3d3-149">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/administrativeunit-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
