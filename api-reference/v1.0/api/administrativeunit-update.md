---
title: Atualizar administrativeunit
description: Atualiza as propriedades de um objeto administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 51eb82bb1bc36e5489a06feed91f34e07422fe16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020192"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="5e645-103">Atualizar administrativeunit</span><span class="sxs-lookup"><span data-stu-id="5e645-103">Update administrativeunit</span></span>

<span data-ttu-id="5e645-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e645-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e645-105">Atualiza as propriedades de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="5e645-105">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e645-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e645-106">Permissions</span></span>
<span data-ttu-id="5e645-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5e645-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e645-109">Permission type</span></span>      | <span data-ttu-id="5e645-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e645-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e645-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e645-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e645-112">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="5e645-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e645-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e645-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e645-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e645-114">Not supported.</span></span>    |
|<span data-ttu-id="5e645-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e645-115">Application</span></span> | <span data-ttu-id="5e645-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e645-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e645-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e645-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /directory/administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5e645-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e645-118">Request headers</span></span>

| <span data-ttu-id="5e645-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5e645-119">Name</span></span>      |<span data-ttu-id="5e645-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e645-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e645-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e645-121">Authorization</span></span>  | <span data-ttu-id="5e645-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e645-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e645-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e645-124">Request body</span></span>

<span data-ttu-id="5e645-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5e645-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e645-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e645-128">Property</span></span>   | <span data-ttu-id="5e645-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e645-129">Type</span></span> |<span data-ttu-id="5e645-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e645-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e645-131">description</span><span class="sxs-lookup"><span data-stu-id="5e645-131">description</span></span>|<span data-ttu-id="5e645-132">string</span><span class="sxs-lookup"><span data-stu-id="5e645-132">string</span></span>|<span data-ttu-id="5e645-133">Descrição da unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="5e645-133">Description for the administrative unit.</span></span>|
|<span data-ttu-id="5e645-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5e645-134">displayName</span></span>|<span data-ttu-id="5e645-135">string</span><span class="sxs-lookup"><span data-stu-id="5e645-135">string</span></span>|<span data-ttu-id="5e645-136">Nome de exibição para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="5e645-136">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="5e645-137">visibilidade</span><span class="sxs-lookup"><span data-stu-id="5e645-137">visibility</span></span>|<span data-ttu-id="5e645-138">string</span><span class="sxs-lookup"><span data-stu-id="5e645-138">string</span></span>|<span data-ttu-id="5e645-139">Visibilidade para a unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="5e645-139">Visibility for the administrative unit.</span></span> <span data-ttu-id="5e645-140">Se não for definido, o padrão será "Public".</span><span class="sxs-lookup"><span data-stu-id="5e645-140">If not set then the default is "public".</span></span> <span data-ttu-id="5e645-141">Pode ser definido como "HiddenMembership", que oculta a associação de não membros.</span><span class="sxs-lookup"><span data-stu-id="5e645-141">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="5e645-142">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode usar a `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância existente do **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="5e645-142">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="5e645-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e645-143">Response</span></span>

<span data-ttu-id="5e645-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5e645-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5e645-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e645-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5e645-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e645-146">Request</span></span>

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

---


##### <a name="response"></a><span data-ttu-id="5e645-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e645-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="5e645-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="5e645-148">See also</span></span>

- [<span data-ttu-id="5e645-149">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="5e645-149">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5e645-150">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="5e645-150">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
