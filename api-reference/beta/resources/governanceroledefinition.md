---
title: tipo de recurso governanceRoleDefinition
description: Representa as definições de função. Para os recursos do Azure, ele pode representar as funções do Azure RBAC, como proprietário, leitor, colaborador, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 668f5430e8f098986b7d5398f32c9c35543a7e11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971848"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="0e9f0-104">tipo de recurso governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0e9f0-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="0e9f0-105">Representa as definições de função.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-105">Represents the role definitions.</span></span> <span data-ttu-id="0e9f0-106">Para os recursos do Azure, ele pode representar as funções do Azure RBAC, como proprietário, leitor, colaborador, etc.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="0e9f0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0e9f0-107">Methods</span></span>

| <span data-ttu-id="0e9f0-108">Método</span><span class="sxs-lookup"><span data-stu-id="0e9f0-108">Method</span></span>          | <span data-ttu-id="0e9f0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e9f0-109">Return Type</span></span> |<span data-ttu-id="0e9f0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e9f0-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="0e9f0-111">List</span><span class="sxs-lookup"><span data-stu-id="0e9f0-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="0e9f0-112">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0e9f0-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="0e9f0-113">Lista uma coleção de definições de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="0e9f0-114">Get</span><span class="sxs-lookup"><span data-stu-id="0e9f0-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="0e9f0-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0e9f0-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="0e9f0-116">Ler propriedades e relações de uma entidade de definição de função especificado por ID.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-116">Read properties and relationships of a role definition entity specified by id.</span></span>|

<span data-ttu-id="0e9f0-117">Não `POST`, `PUT`, `PATCH`, `DELETE` tem suporte no `roleDefinitions` conjunto de entidades por enquanto.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="0e9f0-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e9f0-118">Properties</span></span>
| <span data-ttu-id="0e9f0-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e9f0-119">Property</span></span>  | <span data-ttu-id="0e9f0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e9f0-120">Type</span></span>      |<span data-ttu-id="0e9f0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e9f0-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="0e9f0-122">id</span><span class="sxs-lookup"><span data-stu-id="0e9f0-122">id</span></span>         |<span data-ttu-id="0e9f0-123">String</span><span class="sxs-lookup"><span data-stu-id="0e9f0-123">String</span></span>     |<span data-ttu-id="0e9f0-124">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-124">The id of the role definition.</span></span> |
|<span data-ttu-id="0e9f0-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="0e9f0-125">resourceId</span></span> |<span data-ttu-id="0e9f0-126">String</span><span class="sxs-lookup"><span data-stu-id="0e9f0-126">String</span></span>     |<span data-ttu-id="0e9f0-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-127">Required.</span></span> <span data-ttu-id="0e9f0-128">A ID do recurso associada à definição de função.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="0e9f0-129">externalId</span><span class="sxs-lookup"><span data-stu-id="0e9f0-129">externalId</span></span>   |<span data-ttu-id="0e9f0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e9f0-130">String</span></span>     |<span data-ttu-id="0e9f0-131">A ID externa da definição de função.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="0e9f0-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0e9f0-132">displayName</span></span>|<span data-ttu-id="0e9f0-133">String</span><span class="sxs-lookup"><span data-stu-id="0e9f0-133">String</span></span>     |<span data-ttu-id="0e9f0-134">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="0e9f0-135">templateId</span><span class="sxs-lookup"><span data-stu-id="0e9f0-135">templateId</span></span> | <span data-ttu-id="0e9f0-136">String</span><span class="sxs-lookup"><span data-stu-id="0e9f0-136">String</span></span> | |

## <a name="relationships"></a><span data-ttu-id="0e9f0-137">Relações</span><span class="sxs-lookup"><span data-stu-id="0e9f0-137">Relationships</span></span>
| <span data-ttu-id="0e9f0-138">Relação</span><span class="sxs-lookup"><span data-stu-id="0e9f0-138">Relationship</span></span> | <span data-ttu-id="0e9f0-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e9f0-139">Type</span></span>   |<span data-ttu-id="0e9f0-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e9f0-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e9f0-141">recurso</span><span class="sxs-lookup"><span data-stu-id="0e9f0-141">resource</span></span>|[<span data-ttu-id="0e9f0-142">Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="0e9f0-142">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="0e9f0-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-143">Read-only.</span></span> <span data-ttu-id="0e9f0-144">O recurso associado para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-144">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="0e9f0-145">roleSetting</span><span class="sxs-lookup"><span data-stu-id="0e9f0-145">roleSetting</span></span>|[<span data-ttu-id="0e9f0-146">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="0e9f0-146">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="0e9f0-147">A configuração de função associada para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-147">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e9f0-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e9f0-148">JSON representation</span></span>

<span data-ttu-id="0e9f0-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e9f0-149">Here is a JSON representation of the resource.</span></span>

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
