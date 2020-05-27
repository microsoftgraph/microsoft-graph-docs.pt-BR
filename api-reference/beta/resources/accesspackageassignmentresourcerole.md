---
title: tipo de recurso accessPackageAssignmentResourceRole
description: Uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6ef0827736d16f1dbf3aedfb664467011e75e7b2
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383774"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="5302c-103">tipo de recurso accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="5302c-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="5302c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5302c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5302c-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="5302c-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="5302c-106">Methods</span><span class="sxs-lookup"><span data-stu-id="5302c-106">Methods</span></span>

| <span data-ttu-id="5302c-107">Método</span><span class="sxs-lookup"><span data-stu-id="5302c-107">Method</span></span>       | <span data-ttu-id="5302c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5302c-108">Return Type</span></span> | <span data-ttu-id="5302c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5302c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5302c-110">Obter accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="5302c-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="5302c-111">accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="5302c-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="5302c-112">Recupere um objeto accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="5302c-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="5302c-113">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="5302c-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="5302c-114">coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="5302c-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="5302c-115">Recupere uma lista de objetos accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="5302c-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="5302c-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5302c-116">Properties</span></span>

| <span data-ttu-id="5302c-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5302c-117">Property</span></span>     | <span data-ttu-id="5302c-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="5302c-118">Type</span></span>        | <span data-ttu-id="5302c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5302c-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5302c-120">id</span><span class="sxs-lookup"><span data-stu-id="5302c-120">id</span></span>|<span data-ttu-id="5302c-121">String</span><span class="sxs-lookup"><span data-stu-id="5302c-121">String</span></span>| <span data-ttu-id="5302c-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5302c-122">Read-only.</span></span>|
|<span data-ttu-id="5302c-123">originid</span><span class="sxs-lookup"><span data-stu-id="5302c-123">originId</span></span>|<span data-ttu-id="5302c-124">String</span><span class="sxs-lookup"><span data-stu-id="5302c-124">String</span></span>|<span data-ttu-id="5302c-125">Um identificador exclusivo relativo ao sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="5302c-125">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="5302c-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="5302c-126">originSystem</span></span>|<span data-ttu-id="5302c-127">String</span><span class="sxs-lookup"><span data-stu-id="5302c-127">String</span></span>|<span data-ttu-id="5302c-128">O sistema em que a atribuição de função deve ser criada ou criada para uma atribuição de pacote de acesso, como `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="5302c-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`.</span></span>|
|<span data-ttu-id="5302c-129">status</span><span class="sxs-lookup"><span data-stu-id="5302c-129">status</span></span>|<span data-ttu-id="5302c-130">String</span><span class="sxs-lookup"><span data-stu-id="5302c-130">String</span></span>|<span data-ttu-id="5302c-131">O valor é `Fulfilled` quando a atribuição de pacote de acesso foi entregue ao sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="5302c-131">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5302c-132">Relações</span><span class="sxs-lookup"><span data-stu-id="5302c-132">Relationships</span></span>

| <span data-ttu-id="5302c-133">Relação</span><span class="sxs-lookup"><span data-stu-id="5302c-133">Relationship</span></span> | <span data-ttu-id="5302c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="5302c-134">Type</span></span>        | <span data-ttu-id="5302c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="5302c-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5302c-136">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="5302c-136">accessPackageAssignments</span></span>|<span data-ttu-id="5302c-137">coleção [accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5302c-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="5302c-138">As atribuições de pacote de acesso que resultam nessa atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="5302c-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="5302c-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5302c-139">Read-only.</span></span> <span data-ttu-id="5302c-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5302c-140">Nullable.</span></span>|
|<span data-ttu-id="5302c-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="5302c-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="5302c-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="5302c-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="5302c-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5302c-143">Read-only.</span></span> <span data-ttu-id="5302c-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5302c-144">Nullable.</span></span>|
|<span data-ttu-id="5302c-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="5302c-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="5302c-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="5302c-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="5302c-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5302c-147">Read-only.</span></span> <span data-ttu-id="5302c-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5302c-148">Nullable.</span></span>|
|<span data-ttu-id="5302c-149">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="5302c-149">accessPackageSubject</span></span>|[<span data-ttu-id="5302c-150">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="5302c-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="5302c-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5302c-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5302c-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5302c-153">JSON representation</span></span>

<span data-ttu-id="5302c-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5302c-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
