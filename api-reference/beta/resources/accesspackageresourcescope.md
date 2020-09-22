---
title: tipo de recurso accessPackageResourceScope
description: No gerenciamento de qualificação do Azure AD, um escopo de recurso de pacote do Access é uma referência a um escopo dentro de um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 355838fa9f93cef7d44972b98af317a74036e421
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067521"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="b1e59-103">tipo de recurso accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="b1e59-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="b1e59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1e59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1e59-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um escopo de recurso de pacote do Access é uma referência a um escopo dentro de um recurso, para aqueles recursos que têm vários escopos.</span><span class="sxs-lookup"><span data-stu-id="b1e59-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="b1e59-106">Você pode determinar o escopo de recurso do pacote de acesso para um recurso que já tenha sido adicionado a um pacote do Access, usando [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) para retornar uma coleção de objetos [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="b1e59-106">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="b1e59-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1e59-107">Properties</span></span>

| <span data-ttu-id="b1e59-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1e59-108">Property</span></span>     | <span data-ttu-id="b1e59-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1e59-109">Type</span></span>        | <span data-ttu-id="b1e59-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e59-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1e59-111">description</span><span class="sxs-lookup"><span data-stu-id="b1e59-111">description</span></span>|<span data-ttu-id="b1e59-112">String</span><span class="sxs-lookup"><span data-stu-id="b1e59-112">String</span></span>|<span data-ttu-id="b1e59-113">A descrição do escopo.</span><span class="sxs-lookup"><span data-stu-id="b1e59-113">The description of the scope.</span></span>|
|<span data-ttu-id="b1e59-114">displayName</span><span class="sxs-lookup"><span data-stu-id="b1e59-114">displayName</span></span>|<span data-ttu-id="b1e59-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e59-115">String</span></span>|<span data-ttu-id="b1e59-116">O nome de exibição do escopo.</span><span class="sxs-lookup"><span data-stu-id="b1e59-116">The display name of the scope.</span></span>|
|<span data-ttu-id="b1e59-117">id</span><span class="sxs-lookup"><span data-stu-id="b1e59-117">id</span></span>|<span data-ttu-id="b1e59-118">String</span><span class="sxs-lookup"><span data-stu-id="b1e59-118">String</span></span>| <span data-ttu-id="b1e59-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1e59-119">Read-only.</span></span>|
|<span data-ttu-id="b1e59-120">isRootScope</span><span class="sxs-lookup"><span data-stu-id="b1e59-120">isRootScope</span></span>|<span data-ttu-id="b1e59-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1e59-121">Boolean</span></span>|<span data-ttu-id="b1e59-122">True se os escopos são organizados em uma hierarquia e este é o escopo superior ou raiz do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1e59-122">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="b1e59-123">originid</span><span class="sxs-lookup"><span data-stu-id="b1e59-123">originId</span></span>|<span data-ttu-id="b1e59-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e59-124">String</span></span>|<span data-ttu-id="b1e59-125">O identificador exclusivo do escopo no recurso, conforme definido no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="b1e59-125">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="b1e59-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="b1e59-126">originSystem</span></span>|<span data-ttu-id="b1e59-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e59-127">String</span></span>|<span data-ttu-id="b1e59-128">O sistema de origem para o escopo.</span><span class="sxs-lookup"><span data-stu-id="b1e59-128">The origin system for the scope.</span></span>|
|<span data-ttu-id="b1e59-129">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="b1e59-129">roleOriginId</span></span>|<span data-ttu-id="b1e59-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e59-130">String</span></span>|<span data-ttu-id="b1e59-131">O sistema de origem para a função, se for diferente.</span><span class="sxs-lookup"><span data-stu-id="b1e59-131">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="b1e59-132">url</span><span class="sxs-lookup"><span data-stu-id="b1e59-132">url</span></span>|<span data-ttu-id="b1e59-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e59-133">String</span></span>|<span data-ttu-id="b1e59-134">Um localizador de recursos para o escopo.</span><span class="sxs-lookup"><span data-stu-id="b1e59-134">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1e59-135">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="b1e59-135">Relationships</span></span>

| <span data-ttu-id="b1e59-136">Relação</span><span class="sxs-lookup"><span data-stu-id="b1e59-136">Relationship</span></span> | <span data-ttu-id="b1e59-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1e59-137">Type</span></span>        | <span data-ttu-id="b1e59-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e59-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1e59-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="b1e59-139">accessPackageResource</span></span>|[<span data-ttu-id="b1e59-140">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="b1e59-140">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="b1e59-p101">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b1e59-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1e59-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1e59-143">JSON representation</span></span>

<span data-ttu-id="b1e59-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1e59-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "baseType": "",
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


