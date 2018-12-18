---
title: Atualizar administrativeunit
description: Atualize as propriedades de um objeto administrativeUnit.
author: lleonard-msft
ms.openlocfilehash: 99ec27bc9a60e25d28202d2ebd82155089963c21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362164"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="63d77-103">Atualizar administrativeunit</span><span class="sxs-lookup"><span data-stu-id="63d77-103">Update administrativeunit</span></span>

> <span data-ttu-id="63d77-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63d77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63d77-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63d77-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63d77-106">Atualize as propriedades de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="63d77-106">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="63d77-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="63d77-107">Permissions</span></span>
<span data-ttu-id="63d77-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63d77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="63d77-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63d77-110">Permission type</span></span>      | <span data-ttu-id="63d77-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63d77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63d77-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63d77-112">Delegated (work or school account)</span></span> | <span data-ttu-id="63d77-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63d77-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63d77-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63d77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63d77-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63d77-115">Not supported.</span></span>    |
|<span data-ttu-id="63d77-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63d77-116">Application</span></span> | <span data-ttu-id="63d77-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63d77-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63d77-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63d77-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="63d77-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63d77-119">Request headers</span></span>

| <span data-ttu-id="63d77-120">Nome</span><span class="sxs-lookup"><span data-stu-id="63d77-120">Name</span></span>      |<span data-ttu-id="63d77-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="63d77-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63d77-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63d77-122">Authorization</span></span>  | <span data-ttu-id="63d77-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63d77-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63d77-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63d77-125">Request body</span></span>

<span data-ttu-id="63d77-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="63d77-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="63d77-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63d77-129">Property</span></span>   | <span data-ttu-id="63d77-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="63d77-130">Type</span></span> |<span data-ttu-id="63d77-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="63d77-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63d77-132">description</span><span class="sxs-lookup"><span data-stu-id="63d77-132">description</span></span>|<span data-ttu-id="63d77-133">string</span><span class="sxs-lookup"><span data-stu-id="63d77-133">string</span></span>|<span data-ttu-id="63d77-134">Descrição para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="63d77-134">Description for the administrative unit.</span></span>|
|<span data-ttu-id="63d77-135">displayName</span><span class="sxs-lookup"><span data-stu-id="63d77-135">displayName</span></span>|<span data-ttu-id="63d77-136">string</span><span class="sxs-lookup"><span data-stu-id="63d77-136">string</span></span>|<span data-ttu-id="63d77-137">Nome de exibição para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="63d77-137">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="63d77-138">visibilidade</span><span class="sxs-lookup"><span data-stu-id="63d77-138">visibility</span></span>|<span data-ttu-id="63d77-139">string</span><span class="sxs-lookup"><span data-stu-id="63d77-139">string</span></span>|<span data-ttu-id="63d77-140">Visibilidade para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="63d77-140">Visibility for the administrative unit.</span></span> <span data-ttu-id="63d77-141">Se não estiver definido, então, o padrão é "público".</span><span class="sxs-lookup"><span data-stu-id="63d77-141">If not set then the default is "public".</span></span> <span data-ttu-id="63d77-142">Pode ser definido como "HiddenMembership", que oculta a associação de não-membros.</span><span class="sxs-lookup"><span data-stu-id="63d77-142">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="63d77-143">Desde que o recurso de **administrativeUnit** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância existente do **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="63d77-143">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="63d77-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="63d77-144">Response</span></span>

<span data-ttu-id="63d77-145">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="63d77-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63d77-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63d77-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="63d77-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63d77-147">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="63d77-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="63d77-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="63d77-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="63d77-149">See also</span></span>

- [<span data-ttu-id="63d77-150">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="63d77-150">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="63d77-151">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="63d77-151">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->