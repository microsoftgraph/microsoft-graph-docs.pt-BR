---
title: Tipo de recurso accessPackageResourceScope
description: No gerenciamento de direitos do Azure AD, um escopo de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cd6641b93517f2eadb15e19ef24b35f9f98626fc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158545"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="c7211-103">Tipo de recurso accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="c7211-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="c7211-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7211-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7211-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um escopo de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso, para esses recursos que têm vários escopos.</span><span class="sxs-lookup"><span data-stu-id="c7211-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="c7211-106">Você pode determinar o escopo de recurso do pacote de acesso, para um recurso que já foi adicionado a um pacote de acesso, usando a lista [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) para retornar uma coleção de [objetos accessPackageResourceRoleScope.](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="c7211-106">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="c7211-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7211-107">Properties</span></span>

| <span data-ttu-id="c7211-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7211-108">Property</span></span>     | <span data-ttu-id="c7211-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7211-109">Type</span></span>        | <span data-ttu-id="c7211-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7211-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c7211-111">description</span><span class="sxs-lookup"><span data-stu-id="c7211-111">description</span></span>|<span data-ttu-id="c7211-112">String</span><span class="sxs-lookup"><span data-stu-id="c7211-112">String</span></span>|<span data-ttu-id="c7211-113">A descrição do escopo.</span><span class="sxs-lookup"><span data-stu-id="c7211-113">The description of the scope.</span></span>|
|<span data-ttu-id="c7211-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c7211-114">displayName</span></span>|<span data-ttu-id="c7211-115">String</span><span class="sxs-lookup"><span data-stu-id="c7211-115">String</span></span>|<span data-ttu-id="c7211-116">O nome de exibição do escopo.</span><span class="sxs-lookup"><span data-stu-id="c7211-116">The display name of the scope.</span></span>|
|<span data-ttu-id="c7211-117">id</span><span class="sxs-lookup"><span data-stu-id="c7211-117">id</span></span>|<span data-ttu-id="c7211-118">String</span><span class="sxs-lookup"><span data-stu-id="c7211-118">String</span></span>| <span data-ttu-id="c7211-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7211-119">Read-only.</span></span>|
|<span data-ttu-id="c7211-120">isRootScope</span><span class="sxs-lookup"><span data-stu-id="c7211-120">isRootScope</span></span>|<span data-ttu-id="c7211-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7211-121">Boolean</span></span>|<span data-ttu-id="c7211-122">True se os escopos são organizados em uma hierarquia e este é o escopo superior ou raiz do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7211-122">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="c7211-123">originId</span><span class="sxs-lookup"><span data-stu-id="c7211-123">originId</span></span>|<span data-ttu-id="c7211-124">String</span><span class="sxs-lookup"><span data-stu-id="c7211-124">String</span></span>|<span data-ttu-id="c7211-125">O identificador exclusivo do escopo no recurso, conforme definido no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="c7211-125">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="c7211-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="c7211-126">originSystem</span></span>|<span data-ttu-id="c7211-127">String</span><span class="sxs-lookup"><span data-stu-id="c7211-127">String</span></span>|<span data-ttu-id="c7211-128">O sistema de origem do escopo.</span><span class="sxs-lookup"><span data-stu-id="c7211-128">The origin system for the scope.</span></span>|
|<span data-ttu-id="c7211-129">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="c7211-129">roleOriginId</span></span>|<span data-ttu-id="c7211-130">String</span><span class="sxs-lookup"><span data-stu-id="c7211-130">String</span></span>|<span data-ttu-id="c7211-131">O sistema de origem para a função, se diferente.</span><span class="sxs-lookup"><span data-stu-id="c7211-131">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="c7211-132">url</span><span class="sxs-lookup"><span data-stu-id="c7211-132">url</span></span>|<span data-ttu-id="c7211-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7211-133">String</span></span>|<span data-ttu-id="c7211-134">Um localizador de recursos para o escopo.</span><span class="sxs-lookup"><span data-stu-id="c7211-134">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7211-135">Relações</span><span class="sxs-lookup"><span data-stu-id="c7211-135">Relationships</span></span>

| <span data-ttu-id="c7211-136">Relação</span><span class="sxs-lookup"><span data-stu-id="c7211-136">Relationship</span></span> | <span data-ttu-id="c7211-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7211-137">Type</span></span>        | <span data-ttu-id="c7211-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7211-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c7211-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="c7211-139">accessPackageResource</span></span>|[<span data-ttu-id="c7211-140">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="c7211-140">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="c7211-p101">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c7211-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7211-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7211-143">JSON representation</span></span>

<span data-ttu-id="c7211-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7211-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isRootScope": true,
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


