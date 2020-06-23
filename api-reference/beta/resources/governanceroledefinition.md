---
title: tipo de recurso governanceRoleDefinition
description: Representa as definições de função. Para os recursos do Azure, ele pode representar as funções do Azure RBAC, como proprietário, leitor, colaborador, etc.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1435e8326536aa1a8943e46799d6a5612485a425
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845740"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="63f23-104">tipo de recurso governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="63f23-104">governanceRoleDefinition resource type</span></span>

<span data-ttu-id="63f23-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63f23-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="63f23-106">Representa as definições de função.</span><span class="sxs-lookup"><span data-stu-id="63f23-106">Represents the role definitions.</span></span> <span data-ttu-id="63f23-107">Para os recursos do Azure, ele pode representar as funções do Azure RBAC, como proprietário, leitor, colaborador, etc.</span><span class="sxs-lookup"><span data-stu-id="63f23-107">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="63f23-108">Methods</span><span class="sxs-lookup"><span data-stu-id="63f23-108">Methods</span></span>

| <span data-ttu-id="63f23-109">Método</span><span class="sxs-lookup"><span data-stu-id="63f23-109">Method</span></span>          | <span data-ttu-id="63f23-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="63f23-110">Return Type</span></span> |<span data-ttu-id="63f23-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f23-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="63f23-112">Listar</span><span class="sxs-lookup"><span data-stu-id="63f23-112">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="63f23-113">coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="63f23-113">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="63f23-114">Lista uma coleção de definições de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="63f23-114">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="63f23-115">Get</span><span class="sxs-lookup"><span data-stu-id="63f23-115">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="63f23-116">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="63f23-116">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="63f23-117">Ler propriedades e relações de uma entidade de definição de função especificado por ID.</span><span class="sxs-lookup"><span data-stu-id="63f23-117">Read properties and relationships of a role definition entity specified by id.</span></span>|

<span data-ttu-id="63f23-118">Não `POST` , `PUT` , `PATCH` , `DELETE` tem suporte no `roleDefinitions` conjunto de entidades por enquanto.</span><span class="sxs-lookup"><span data-stu-id="63f23-118">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="63f23-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63f23-119">Properties</span></span>
| <span data-ttu-id="63f23-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63f23-120">Property</span></span>    | <span data-ttu-id="63f23-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="63f23-121">Type</span></span>   | <span data-ttu-id="63f23-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f23-122">Description</span></span>                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| <span data-ttu-id="63f23-123">id</span><span class="sxs-lookup"><span data-stu-id="63f23-123">id</span></span>          | <span data-ttu-id="63f23-124">String</span><span class="sxs-lookup"><span data-stu-id="63f23-124">String</span></span> | <span data-ttu-id="63f23-125">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="63f23-125">The id of the role definition.</span></span>                                        |
| <span data-ttu-id="63f23-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="63f23-126">resourceId</span></span>  | <span data-ttu-id="63f23-127">String</span><span class="sxs-lookup"><span data-stu-id="63f23-127">String</span></span> | <span data-ttu-id="63f23-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63f23-128">Required.</span></span> <span data-ttu-id="63f23-129">A ID do recurso associada à definição de função.</span><span class="sxs-lookup"><span data-stu-id="63f23-129">The id of the resource associated with the role definition.</span></span> |
| <span data-ttu-id="63f23-130">externalId</span><span class="sxs-lookup"><span data-stu-id="63f23-130">externalId</span></span>  | <span data-ttu-id="63f23-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63f23-131">String</span></span> | <span data-ttu-id="63f23-132">A ID externa da definição de função.</span><span class="sxs-lookup"><span data-stu-id="63f23-132">The external id of the role definition.</span></span>                               |
| <span data-ttu-id="63f23-133">displayName</span><span class="sxs-lookup"><span data-stu-id="63f23-133">displayName</span></span> | <span data-ttu-id="63f23-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63f23-134">String</span></span> | <span data-ttu-id="63f23-135">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="63f23-135">The display name of the role definition.</span></span>                              |
| <span data-ttu-id="63f23-136">templateId</span><span class="sxs-lookup"><span data-stu-id="63f23-136">templateId</span></span>  | <span data-ttu-id="63f23-137">String</span><span class="sxs-lookup"><span data-stu-id="63f23-137">String</span></span> |                                                                       |

## <a name="relationships"></a><span data-ttu-id="63f23-138">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="63f23-138">Relationships</span></span>
| <span data-ttu-id="63f23-139">Relação</span><span class="sxs-lookup"><span data-stu-id="63f23-139">Relationship</span></span> | <span data-ttu-id="63f23-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="63f23-140">Type</span></span>   |<span data-ttu-id="63f23-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f23-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63f23-142">recurso</span><span class="sxs-lookup"><span data-stu-id="63f23-142">resource</span></span>|[<span data-ttu-id="63f23-143">governanceResource</span><span class="sxs-lookup"><span data-stu-id="63f23-143">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="63f23-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63f23-144">Read-only.</span></span> <span data-ttu-id="63f23-145">O recurso associado para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="63f23-145">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="63f23-146">roleSetting</span><span class="sxs-lookup"><span data-stu-id="63f23-146">roleSetting</span></span>|[<span data-ttu-id="63f23-147">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="63f23-147">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="63f23-148">A configuração de função associada para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="63f23-148">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63f23-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63f23-149">JSON representation</span></span>

<span data-ttu-id="63f23-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63f23-150">Here is a JSON representation of the resource.</span></span>

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
