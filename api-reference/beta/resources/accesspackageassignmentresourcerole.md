---
title: tipo de recurso accessPackageAssignmentResourceRole
description: Uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8bf839d68db3f54df5a27601a4a05463e013fbef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089858"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="73856-103">tipo de recurso accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="73856-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="73856-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73856-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73856-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="73856-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="73856-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="73856-106">Methods</span></span>

| <span data-ttu-id="73856-107">Método</span><span class="sxs-lookup"><span data-stu-id="73856-107">Method</span></span>       | <span data-ttu-id="73856-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73856-108">Return Type</span></span> | <span data-ttu-id="73856-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73856-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="73856-110">Obter accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="73856-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="73856-111">accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="73856-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="73856-112">Recupere um objeto accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="73856-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="73856-113">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="73856-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="73856-114">coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="73856-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="73856-115">Recupere uma lista de objetos accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="73856-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="73856-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73856-116">Properties</span></span>

| <span data-ttu-id="73856-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73856-117">Property</span></span>     | <span data-ttu-id="73856-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="73856-118">Type</span></span>        | <span data-ttu-id="73856-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="73856-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73856-120">id</span><span class="sxs-lookup"><span data-stu-id="73856-120">id</span></span>|<span data-ttu-id="73856-121">String</span><span class="sxs-lookup"><span data-stu-id="73856-121">String</span></span>| <span data-ttu-id="73856-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73856-122">Read-only.</span></span>|
|<span data-ttu-id="73856-123">originid</span><span class="sxs-lookup"><span data-stu-id="73856-123">originId</span></span>|<span data-ttu-id="73856-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73856-124">String</span></span>|<span data-ttu-id="73856-125">Um identificador exclusivo relativo ao sistema de origem, correspondente à propriedade originid do [accessPackageResourceRole](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="73856-125">A unique identifier relative to the origin system, corresponding to the originId property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span> |
|<span data-ttu-id="73856-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="73856-126">originSystem</span></span>|<span data-ttu-id="73856-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73856-127">String</span></span>|<span data-ttu-id="73856-128">O sistema em que a atribuição de função deve ser criada ou criada para uma atribuição de pacote de acesso, como `SharePointOnline` , `AadGroup` ou `AadApplication` , correspondente à propriedade originSystem do [accessPackageResourceRole](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="73856-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`, `AadGroup` or `AadApplication`, corresponding to the originSystem property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span>|
|<span data-ttu-id="73856-129">status</span><span class="sxs-lookup"><span data-stu-id="73856-129">status</span></span>|<span data-ttu-id="73856-130">String</span><span class="sxs-lookup"><span data-stu-id="73856-130">String</span></span>|<span data-ttu-id="73856-131">O valor é `PendingFulfillment` quando a atribuição de pacote de acesso ainda não foi entregue ao sistema de origem e `Fulfilled` quando a atribuição de pacote de acesso foi entregue ao sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="73856-131">The value is `PendingFulfillment` when the access package assignment has not yet been delivered to the origin system, and `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73856-132">Relações</span><span class="sxs-lookup"><span data-stu-id="73856-132">Relationships</span></span>

| <span data-ttu-id="73856-133">Relação</span><span class="sxs-lookup"><span data-stu-id="73856-133">Relationship</span></span> | <span data-ttu-id="73856-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="73856-134">Type</span></span>        | <span data-ttu-id="73856-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="73856-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73856-136">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="73856-136">accessPackageAssignments</span></span>|<span data-ttu-id="73856-137">coleção [accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="73856-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="73856-138">As atribuições de pacote de acesso que resultam nessa atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="73856-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="73856-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73856-139">Read-only.</span></span> <span data-ttu-id="73856-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73856-140">Nullable.</span></span>|
|<span data-ttu-id="73856-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="73856-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="73856-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="73856-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="73856-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73856-143">Read-only.</span></span> <span data-ttu-id="73856-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73856-144">Nullable.</span></span>|
|<span data-ttu-id="73856-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="73856-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="73856-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="73856-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="73856-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73856-147">Read-only.</span></span> <span data-ttu-id="73856-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73856-148">Nullable.</span></span>|
|<span data-ttu-id="73856-149">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="73856-149">accessPackageSubject</span></span>|[<span data-ttu-id="73856-150">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="73856-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="73856-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="73856-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="73856-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73856-153">JSON representation</span></span>

<span data-ttu-id="73856-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73856-154">The following is a JSON representation of the resource.</span></span>

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


