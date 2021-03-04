---
title: Tipo de recurso accessPackageAssignmentResourceRole
description: Uma função de recurso de atribuição de pacote de acesso indica a função específica do recurso que um assunto foi atribuído por meio de uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4473c303a74cbf9e8e0c17d6c9060960590a3405
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433262"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="2bcef-103">Tipo de recurso accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="2bcef-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="2bcef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bcef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bcef-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma função de recurso de atribuição de pacote de acesso indica a função específica do recurso que um assunto foi atribuído por meio de uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="2bcef-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="2bcef-106">Methods</span><span class="sxs-lookup"><span data-stu-id="2bcef-106">Methods</span></span>

| <span data-ttu-id="2bcef-107">Método</span><span class="sxs-lookup"><span data-stu-id="2bcef-107">Method</span></span>       | <span data-ttu-id="2bcef-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2bcef-108">Return Type</span></span> | <span data-ttu-id="2bcef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcef-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2bcef-110">Obter accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="2bcef-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="2bcef-111">accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="2bcef-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="2bcef-112">Recupere um objeto accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="2bcef-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="2bcef-113">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="2bcef-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="2bcef-114">[Coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="2bcef-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="2bcef-115">Recupere uma lista de objetos accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="2bcef-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="2bcef-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bcef-116">Properties</span></span>

| <span data-ttu-id="2bcef-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bcef-117">Property</span></span>     | <span data-ttu-id="2bcef-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bcef-118">Type</span></span>        | <span data-ttu-id="2bcef-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcef-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bcef-120">id</span><span class="sxs-lookup"><span data-stu-id="2bcef-120">id</span></span>|<span data-ttu-id="2bcef-121">String</span><span class="sxs-lookup"><span data-stu-id="2bcef-121">String</span></span>| <span data-ttu-id="2bcef-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bcef-122">Read-only.</span></span>|
|<span data-ttu-id="2bcef-123">originId</span><span class="sxs-lookup"><span data-stu-id="2bcef-123">originId</span></span>|<span data-ttu-id="2bcef-124">String</span><span class="sxs-lookup"><span data-stu-id="2bcef-124">String</span></span>|<span data-ttu-id="2bcef-125">Um identificador exclusivo em relação ao sistema de origem, correspondente à propriedade originId do [accessPackageResourceRole](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="2bcef-125">A unique identifier relative to the origin system, corresponding to the originId property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span> |
|<span data-ttu-id="2bcef-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="2bcef-126">originSystem</span></span>|<span data-ttu-id="2bcef-127">String</span><span class="sxs-lookup"><span data-stu-id="2bcef-127">String</span></span>|<span data-ttu-id="2bcef-128">O sistema onde a atribuição de função deve ser criada ou foi criada para uma atribuição de pacote de acesso, como , ou , correspondente à propriedade originSystem do `SharePointOnline` `AadGroup` `AadApplication` [accessPackageResourceRole](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="2bcef-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`, `AadGroup` or `AadApplication`, corresponding to the originSystem property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span>|
|<span data-ttu-id="2bcef-129">status</span><span class="sxs-lookup"><span data-stu-id="2bcef-129">status</span></span>|<span data-ttu-id="2bcef-130">String</span><span class="sxs-lookup"><span data-stu-id="2bcef-130">String</span></span>|<span data-ttu-id="2bcef-131">O valor é quando a atribuição do pacote de acesso ainda não foi entregue ao sistema de origem e quando a atribuição do pacote de acesso foi entregue `PendingFulfillment` `Fulfilled` ao sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="2bcef-131">The value is `PendingFulfillment` when the access package assignment has not yet been delivered to the origin system, and `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bcef-132">Relações</span><span class="sxs-lookup"><span data-stu-id="2bcef-132">Relationships</span></span>

| <span data-ttu-id="2bcef-133">Relação</span><span class="sxs-lookup"><span data-stu-id="2bcef-133">Relationship</span></span> | <span data-ttu-id="2bcef-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bcef-134">Type</span></span>        | <span data-ttu-id="2bcef-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcef-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bcef-136">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="2bcef-136">accessPackageAssignments</span></span>|<span data-ttu-id="2bcef-137">[Coleção accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2bcef-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="2bcef-138">As atribuições do pacote de acesso resultantes dessa atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="2bcef-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="2bcef-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bcef-139">Read-only.</span></span> <span data-ttu-id="2bcef-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2bcef-140">Nullable.</span></span>|
|<span data-ttu-id="2bcef-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="2bcef-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="2bcef-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="2bcef-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="2bcef-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bcef-143">Read-only.</span></span> <span data-ttu-id="2bcef-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2bcef-144">Nullable.</span></span>|
|<span data-ttu-id="2bcef-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="2bcef-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="2bcef-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="2bcef-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="2bcef-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bcef-147">Read-only.</span></span> <span data-ttu-id="2bcef-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2bcef-148">Nullable.</span></span>|
|<span data-ttu-id="2bcef-149">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="2bcef-149">accessPackageSubject</span></span>|[<span data-ttu-id="2bcef-150">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="2bcef-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="2bcef-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2bcef-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2bcef-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bcef-153">JSON representation</span></span>

<span data-ttu-id="2bcef-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bcef-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
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


