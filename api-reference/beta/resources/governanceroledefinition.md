---
title: Tipo de recurso governanceRoleDefinition
description: Representa as definições de função. Para recursos do Azure, ele pode representar funções do Azure RBAC, como Proprietário, Leitor, Colaborador, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: dd4a9fc90d3c12669464a5e9b931b968d4526640
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443052"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="11e0f-104">Tipo de recurso governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="11e0f-104">governanceRoleDefinition resource type</span></span>

<span data-ttu-id="11e0f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11e0f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="11e0f-106">Representa as definições de função.</span><span class="sxs-lookup"><span data-stu-id="11e0f-106">Represents the role definitions.</span></span> <span data-ttu-id="11e0f-107">Para recursos do Azure, ele pode representar funções do Azure RBAC, como Proprietário, Leitor, Colaborador, etc.</span><span class="sxs-lookup"><span data-stu-id="11e0f-107">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="11e0f-108">Methods</span><span class="sxs-lookup"><span data-stu-id="11e0f-108">Methods</span></span>

| <span data-ttu-id="11e0f-109">Método</span><span class="sxs-lookup"><span data-stu-id="11e0f-109">Method</span></span>          | <span data-ttu-id="11e0f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="11e0f-110">Return Type</span></span> |<span data-ttu-id="11e0f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11e0f-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="11e0f-112">List</span><span class="sxs-lookup"><span data-stu-id="11e0f-112">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="11e0f-113">[Coleção governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11e0f-113">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="11e0f-114">Listar uma coleção de definições de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="11e0f-114">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="11e0f-115">Get</span><span class="sxs-lookup"><span data-stu-id="11e0f-115">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="11e0f-116">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="11e0f-116">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="11e0f-117">Ler propriedades e relações de uma entidade de definição de função especificada pela id.</span><span class="sxs-lookup"><span data-stu-id="11e0f-117">Read properties and relationships of a role definition entity specified by id.</span></span>|

<span data-ttu-id="11e0f-118">Não `POST` , , é suportado no conjunto de `PUT` `PATCH` `DELETE` `roleDefinitions` entidades por enquanto.</span><span class="sxs-lookup"><span data-stu-id="11e0f-118">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="11e0f-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11e0f-119">Properties</span></span>
| <span data-ttu-id="11e0f-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11e0f-120">Property</span></span>    | <span data-ttu-id="11e0f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="11e0f-121">Type</span></span>   | <span data-ttu-id="11e0f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="11e0f-122">Description</span></span>                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| <span data-ttu-id="11e0f-123">id</span><span class="sxs-lookup"><span data-stu-id="11e0f-123">id</span></span>          | <span data-ttu-id="11e0f-124">String</span><span class="sxs-lookup"><span data-stu-id="11e0f-124">String</span></span> | <span data-ttu-id="11e0f-125">A id da definição de função.</span><span class="sxs-lookup"><span data-stu-id="11e0f-125">The id of the role definition.</span></span>                                        |
| <span data-ttu-id="11e0f-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="11e0f-126">resourceId</span></span>  | <span data-ttu-id="11e0f-127">String</span><span class="sxs-lookup"><span data-stu-id="11e0f-127">String</span></span> | <span data-ttu-id="11e0f-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11e0f-128">Required.</span></span> <span data-ttu-id="11e0f-129">A id do recurso associado à definição de função.</span><span class="sxs-lookup"><span data-stu-id="11e0f-129">The id of the resource associated with the role definition.</span></span> |
| <span data-ttu-id="11e0f-130">externalId</span><span class="sxs-lookup"><span data-stu-id="11e0f-130">externalId</span></span>  | <span data-ttu-id="11e0f-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11e0f-131">String</span></span> | <span data-ttu-id="11e0f-132">A id externa da definição de função.</span><span class="sxs-lookup"><span data-stu-id="11e0f-132">The external id of the role definition.</span></span>                               |
| <span data-ttu-id="11e0f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="11e0f-133">displayName</span></span> | <span data-ttu-id="11e0f-134">String</span><span class="sxs-lookup"><span data-stu-id="11e0f-134">String</span></span> | <span data-ttu-id="11e0f-135">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="11e0f-135">The display name of the role definition.</span></span>                              |
| <span data-ttu-id="11e0f-136">templateId</span><span class="sxs-lookup"><span data-stu-id="11e0f-136">templateId</span></span>  | <span data-ttu-id="11e0f-137">String</span><span class="sxs-lookup"><span data-stu-id="11e0f-137">String</span></span> |                                                                       |

## <a name="relationships"></a><span data-ttu-id="11e0f-138">Relações</span><span class="sxs-lookup"><span data-stu-id="11e0f-138">Relationships</span></span>
| <span data-ttu-id="11e0f-139">Relação</span><span class="sxs-lookup"><span data-stu-id="11e0f-139">Relationship</span></span> | <span data-ttu-id="11e0f-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="11e0f-140">Type</span></span>   |<span data-ttu-id="11e0f-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="11e0f-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11e0f-142">recurso</span><span class="sxs-lookup"><span data-stu-id="11e0f-142">resource</span></span>|[<span data-ttu-id="11e0f-143">governanceResource</span><span class="sxs-lookup"><span data-stu-id="11e0f-143">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="11e0f-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11e0f-144">Read-only.</span></span> <span data-ttu-id="11e0f-145">O recurso associado para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="11e0f-145">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="11e0f-146">roleSetting</span><span class="sxs-lookup"><span data-stu-id="11e0f-146">roleSetting</span></span>|[<span data-ttu-id="11e0f-147">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="11e0f-147">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="11e0f-148">A configuração de função associada para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="11e0f-148">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11e0f-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11e0f-149">JSON representation</span></span>

<span data-ttu-id="11e0f-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11e0f-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
  "templateId":"String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


