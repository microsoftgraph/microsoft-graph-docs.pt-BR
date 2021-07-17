---
title: Tipo de recurso accessPackageResourceScope
description: No gerenciamento de direitos do Azure AD, um escopo de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6da0211cad6dcca225f4c9848216eda2deaf7b0a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467173"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="42a83-103">Tipo de recurso accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="42a83-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="42a83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42a83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42a83-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um escopo de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso, para esses recursos que têm vários escopos.</span><span class="sxs-lookup"><span data-stu-id="42a83-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="42a83-106">Você pode determinar o escopo de recurso do pacote de acesso, para um recurso que já tenha funções adicionadas a um pacote de acesso, usando [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) de lista para retornar uma coleção de objetos [accessPackageResourceRoleScope.](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="42a83-106">You can determine the access package resource scope, for a resource which has roles already added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

<span data-ttu-id="42a83-107">Se o recurso estiver em um catálogo de pacotes de acesso, mas ainda não tiver suas funções adicionadas a um pacote de acesso, você poderá determinar o escopo de recurso do pacote de acesso usando o [accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) de lista e incluindo na `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` consulta.</span><span class="sxs-lookup"><span data-stu-id="42a83-107">If the resource is in an access package catalog but has not yet had its roles added to an access package, you can determine the access package resource scope by using [list accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) and including `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` in the query.</span></span>

## <a name="properties"></a><span data-ttu-id="42a83-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42a83-108">Properties</span></span>

| <span data-ttu-id="42a83-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42a83-109">Property</span></span>     | <span data-ttu-id="42a83-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="42a83-110">Type</span></span>        | <span data-ttu-id="42a83-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42a83-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42a83-112">description</span><span class="sxs-lookup"><span data-stu-id="42a83-112">description</span></span>|<span data-ttu-id="42a83-113">String</span><span class="sxs-lookup"><span data-stu-id="42a83-113">String</span></span>|<span data-ttu-id="42a83-114">A descrição do escopo.</span><span class="sxs-lookup"><span data-stu-id="42a83-114">The description of the scope.</span></span>|
|<span data-ttu-id="42a83-115">displayName</span><span class="sxs-lookup"><span data-stu-id="42a83-115">displayName</span></span>|<span data-ttu-id="42a83-116">String</span><span class="sxs-lookup"><span data-stu-id="42a83-116">String</span></span>|<span data-ttu-id="42a83-117">O nome de exibição do escopo.</span><span class="sxs-lookup"><span data-stu-id="42a83-117">The display name of the scope.</span></span>|
|<span data-ttu-id="42a83-118">id</span><span class="sxs-lookup"><span data-stu-id="42a83-118">id</span></span>|<span data-ttu-id="42a83-119">String</span><span class="sxs-lookup"><span data-stu-id="42a83-119">String</span></span>| <span data-ttu-id="42a83-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42a83-120">Read-only.</span></span>|
|<span data-ttu-id="42a83-121">isRootScope</span><span class="sxs-lookup"><span data-stu-id="42a83-121">isRootScope</span></span>|<span data-ttu-id="42a83-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="42a83-122">Boolean</span></span>|<span data-ttu-id="42a83-123">True se os escopos são organizados em uma hierarquia e este é o escopo superior ou raiz do recurso.</span><span class="sxs-lookup"><span data-stu-id="42a83-123">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="42a83-124">originId</span><span class="sxs-lookup"><span data-stu-id="42a83-124">originId</span></span>|<span data-ttu-id="42a83-125">String</span><span class="sxs-lookup"><span data-stu-id="42a83-125">String</span></span>|<span data-ttu-id="42a83-126">O identificador exclusivo do escopo no recurso conforme definido no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="42a83-126">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="42a83-127">originSystem</span><span class="sxs-lookup"><span data-stu-id="42a83-127">originSystem</span></span>|<span data-ttu-id="42a83-128">String</span><span class="sxs-lookup"><span data-stu-id="42a83-128">String</span></span>|<span data-ttu-id="42a83-129">O sistema de origem do escopo.</span><span class="sxs-lookup"><span data-stu-id="42a83-129">The origin system for the scope.</span></span>|
|<span data-ttu-id="42a83-130">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="42a83-130">roleOriginId</span></span>|<span data-ttu-id="42a83-131">String</span><span class="sxs-lookup"><span data-stu-id="42a83-131">String</span></span>|<span data-ttu-id="42a83-132">O sistema de origem da função, se diferente.</span><span class="sxs-lookup"><span data-stu-id="42a83-132">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="42a83-133">url</span><span class="sxs-lookup"><span data-stu-id="42a83-133">url</span></span>|<span data-ttu-id="42a83-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42a83-134">String</span></span>|<span data-ttu-id="42a83-135">Um localizador de recursos para o escopo.</span><span class="sxs-lookup"><span data-stu-id="42a83-135">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42a83-136">Relações</span><span class="sxs-lookup"><span data-stu-id="42a83-136">Relationships</span></span>

| <span data-ttu-id="42a83-137">Relação</span><span class="sxs-lookup"><span data-stu-id="42a83-137">Relationship</span></span> | <span data-ttu-id="42a83-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="42a83-138">Type</span></span>        | <span data-ttu-id="42a83-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="42a83-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42a83-140">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="42a83-140">accessPackageResource</span></span>|[<span data-ttu-id="42a83-141">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="42a83-141">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="42a83-p101">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="42a83-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42a83-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42a83-144">JSON representation</span></span>

<span data-ttu-id="42a83-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42a83-145">The following is a JSON representation of the resource.</span></span>

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


