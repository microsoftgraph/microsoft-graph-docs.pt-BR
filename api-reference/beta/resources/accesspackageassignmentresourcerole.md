---
title: tipo de recurso accessPackageAssignmentResourceRole
description: Uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eddff042af5b2cd724e87e3438f398e8d68c19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508538"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="6d1d4-103">tipo de recurso accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="6d1d4-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="6d1d4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6d1d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d1d4-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="6d1d4-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6d1d4-106">Methods</span></span>

| <span data-ttu-id="6d1d4-107">Método</span><span class="sxs-lookup"><span data-stu-id="6d1d4-107">Method</span></span>       | <span data-ttu-id="6d1d4-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6d1d4-108">Return Type</span></span> | <span data-ttu-id="6d1d4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d1d4-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6d1d4-110">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="6d1d4-110">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="6d1d4-111">coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="6d1d4-111">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="6d1d4-112">Recupere uma lista de objetos accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-112">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="6d1d4-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d1d4-113">Properties</span></span>

| <span data-ttu-id="6d1d4-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d1d4-114">Property</span></span>     | <span data-ttu-id="6d1d4-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d1d4-115">Type</span></span>        | <span data-ttu-id="6d1d4-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d1d4-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d1d4-117">id</span><span class="sxs-lookup"><span data-stu-id="6d1d4-117">id</span></span>|<span data-ttu-id="6d1d4-118">String</span><span class="sxs-lookup"><span data-stu-id="6d1d4-118">String</span></span>| <span data-ttu-id="6d1d4-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-119">Read-only.</span></span>|
|<span data-ttu-id="6d1d4-120">originid</span><span class="sxs-lookup"><span data-stu-id="6d1d4-120">originId</span></span>|<span data-ttu-id="6d1d4-121">String</span><span class="sxs-lookup"><span data-stu-id="6d1d4-121">String</span></span>|<span data-ttu-id="6d1d4-122">Um identificador exclusivo relativo ao sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-122">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="6d1d4-123">originSystem</span><span class="sxs-lookup"><span data-stu-id="6d1d4-123">originSystem</span></span>|<span data-ttu-id="6d1d4-124">String</span><span class="sxs-lookup"><span data-stu-id="6d1d4-124">String</span></span>|<span data-ttu-id="6d1d4-125">O sistema em que a atribuição de função deve ser criada para uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-125">The system where the role assignment is to be created for an access package assignment.</span></span>|
|<span data-ttu-id="6d1d4-126">status</span><span class="sxs-lookup"><span data-stu-id="6d1d4-126">status</span></span>|<span data-ttu-id="6d1d4-127">String</span><span class="sxs-lookup"><span data-stu-id="6d1d4-127">String</span></span>|<span data-ttu-id="6d1d4-128">O valor é `Fulfilled` quando a atribuição de pacote de acesso foi entregue ao sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-128">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d1d4-129">Relações</span><span class="sxs-lookup"><span data-stu-id="6d1d4-129">Relationships</span></span>

| <span data-ttu-id="6d1d4-130">Relação</span><span class="sxs-lookup"><span data-stu-id="6d1d4-130">Relationship</span></span> | <span data-ttu-id="6d1d4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d1d4-131">Type</span></span>        | <span data-ttu-id="6d1d4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d1d4-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d1d4-133">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="6d1d4-133">accessPackageAssignments</span></span>|<span data-ttu-id="6d1d4-134">coleção [accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6d1d4-134">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="6d1d4-135">As atribuições de pacote de acesso que resultam nessa atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-135">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="6d1d4-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-136">Read-only.</span></span> <span data-ttu-id="6d1d4-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-137">Nullable.</span></span>|
|<span data-ttu-id="6d1d4-138">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="6d1d4-138">accessPackageResourceRole</span></span>|[<span data-ttu-id="6d1d4-139">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="6d1d4-139">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="6d1d4-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-140">Read-only.</span></span> <span data-ttu-id="6d1d4-141">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-141">Nullable.</span></span>|
|<span data-ttu-id="6d1d4-142">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="6d1d4-142">accessPackageResourceScope</span></span>|[<span data-ttu-id="6d1d4-143">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="6d1d4-143">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="6d1d4-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-144">Read-only.</span></span> <span data-ttu-id="6d1d4-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-145">Nullable.</span></span>|
|<span data-ttu-id="6d1d4-146">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="6d1d4-146">accessPackageSubject</span></span>|[<span data-ttu-id="6d1d4-147">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="6d1d4-147">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="6d1d4-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6d1d4-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d1d4-150">JSON representation</span></span>

<span data-ttu-id="6d1d4-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d1d4-151">The following is a JSON representation of the resource.</span></span>

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
