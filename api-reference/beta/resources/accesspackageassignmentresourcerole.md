---
title: tipo de recurso accessPackageAssignmentResourceRole
description: Uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1dbf73623ddd51cc1172e5610e84cc7861657489
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939191"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="987a3-103">tipo de recurso accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="987a3-103">accessPackageAssignmentResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="987a3-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="987a3-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="987a3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="987a3-105">Methods</span></span>

| <span data-ttu-id="987a3-106">Método</span><span class="sxs-lookup"><span data-stu-id="987a3-106">Method</span></span>       | <span data-ttu-id="987a3-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="987a3-107">Return Type</span></span> | <span data-ttu-id="987a3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="987a3-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="987a3-109">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="987a3-109">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="987a3-110">coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="987a3-110">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="987a3-111">Recupere uma lista de objetos accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="987a3-111">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="987a3-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="987a3-112">Properties</span></span>

| <span data-ttu-id="987a3-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="987a3-113">Property</span></span>     | <span data-ttu-id="987a3-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="987a3-114">Type</span></span>        | <span data-ttu-id="987a3-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="987a3-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="987a3-116">id</span><span class="sxs-lookup"><span data-stu-id="987a3-116">id</span></span>|<span data-ttu-id="987a3-117">String</span><span class="sxs-lookup"><span data-stu-id="987a3-117">String</span></span>| <span data-ttu-id="987a3-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="987a3-118">Read-only.</span></span>|
|<span data-ttu-id="987a3-119">originid</span><span class="sxs-lookup"><span data-stu-id="987a3-119">originId</span></span>|<span data-ttu-id="987a3-120">String</span><span class="sxs-lookup"><span data-stu-id="987a3-120">String</span></span>|<span data-ttu-id="987a3-121">Um identificador exclusivo relativo ao sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="987a3-121">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="987a3-122">originSystem</span><span class="sxs-lookup"><span data-stu-id="987a3-122">originSystem</span></span>|<span data-ttu-id="987a3-123">String</span><span class="sxs-lookup"><span data-stu-id="987a3-123">String</span></span>|<span data-ttu-id="987a3-124">O sistema em que a atribuição de função deve ser criada para uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="987a3-124">The system where the role assignment is to be created for an access package assignment.</span></span>|
|<span data-ttu-id="987a3-125">status</span><span class="sxs-lookup"><span data-stu-id="987a3-125">status</span></span>|<span data-ttu-id="987a3-126">String</span><span class="sxs-lookup"><span data-stu-id="987a3-126">String</span></span>|<span data-ttu-id="987a3-127">O valor é `Fulfilled` quando a atribuição de pacote de acesso foi entregue ao sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="987a3-127">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="987a3-128">Relações</span><span class="sxs-lookup"><span data-stu-id="987a3-128">Relationships</span></span>

| <span data-ttu-id="987a3-129">Relação</span><span class="sxs-lookup"><span data-stu-id="987a3-129">Relationship</span></span> | <span data-ttu-id="987a3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="987a3-130">Type</span></span>        | <span data-ttu-id="987a3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="987a3-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="987a3-132">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="987a3-132">accessPackageAssignments</span></span>|<span data-ttu-id="987a3-133">coleção [accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="987a3-133">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="987a3-134">As atribuições de pacote de acesso que resultam nessa atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="987a3-134">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="987a3-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="987a3-135">Read-only.</span></span> <span data-ttu-id="987a3-136">Anulável.</span><span class="sxs-lookup"><span data-stu-id="987a3-136">Nullable.</span></span>|
|<span data-ttu-id="987a3-137">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="987a3-137">accessPackageResourceRole</span></span>|[<span data-ttu-id="987a3-138">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="987a3-138">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="987a3-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="987a3-139">Read-only.</span></span> <span data-ttu-id="987a3-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="987a3-140">Nullable.</span></span>|
|<span data-ttu-id="987a3-141">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="987a3-141">accessPackageResourceScope</span></span>|[<span data-ttu-id="987a3-142">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="987a3-142">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="987a3-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="987a3-143">Read-only.</span></span> <span data-ttu-id="987a3-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="987a3-144">Nullable.</span></span>|
|<span data-ttu-id="987a3-145">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="987a3-145">accessPackageSubject</span></span>|[<span data-ttu-id="987a3-146">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="987a3-146">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="987a3-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="987a3-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="987a3-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="987a3-149">JSON representation</span></span>

<span data-ttu-id="987a3-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="987a3-150">The following is a JSON representation of the resource.</span></span>

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
