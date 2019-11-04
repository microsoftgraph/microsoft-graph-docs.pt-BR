---
title: tipo de recurso accessPackageResourceScope
description: No gerenciamento de qualificação do Azure AD, um escopo de recurso de pacote do Access é uma referência a um escopo dentro de um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7bfa2f617e746aee17a62a7550c41e3de54f47cd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939513"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="f9ce0-103">tipo de recurso accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="f9ce0-103">accessPackageResourceScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9ce0-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um escopo de recurso de pacote do Access é uma referência a um escopo dentro de um recurso, para aqueles recursos que têm vários escopos.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="f9ce0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9ce0-105">Properties</span></span>

| <span data-ttu-id="f9ce0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9ce0-106">Property</span></span>     | <span data-ttu-id="f9ce0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9ce0-107">Type</span></span>        | <span data-ttu-id="f9ce0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9ce0-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f9ce0-109">description</span><span class="sxs-lookup"><span data-stu-id="f9ce0-109">description</span></span>|<span data-ttu-id="f9ce0-110">String</span><span class="sxs-lookup"><span data-stu-id="f9ce0-110">String</span></span>|<span data-ttu-id="f9ce0-111">A descrição do escopo.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-111">The description of the scope.</span></span>|
|<span data-ttu-id="f9ce0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f9ce0-112">displayName</span></span>|<span data-ttu-id="f9ce0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9ce0-113">String</span></span>|<span data-ttu-id="f9ce0-114">O nome de exibição do escopo.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-114">The display name of the scope.</span></span>|
|<span data-ttu-id="f9ce0-115">id</span><span class="sxs-lookup"><span data-stu-id="f9ce0-115">id</span></span>|<span data-ttu-id="f9ce0-116">String</span><span class="sxs-lookup"><span data-stu-id="f9ce0-116">String</span></span>| <span data-ttu-id="f9ce0-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-117">Read-only.</span></span>|
|<span data-ttu-id="f9ce0-118">isRootScope</span><span class="sxs-lookup"><span data-stu-id="f9ce0-118">isRootScope</span></span>|<span data-ttu-id="f9ce0-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9ce0-119">Boolean</span></span>|<span data-ttu-id="f9ce0-120">True se os escopos são organizados em uma hierarquia e este é o escopo superior ou raiz do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-120">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="f9ce0-121">originid</span><span class="sxs-lookup"><span data-stu-id="f9ce0-121">originId</span></span>|<span data-ttu-id="f9ce0-122">String</span><span class="sxs-lookup"><span data-stu-id="f9ce0-122">String</span></span>|<span data-ttu-id="f9ce0-123">O identificador exclusivo do escopo no recurso, conforme definido no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-123">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="f9ce0-124">originSystem</span><span class="sxs-lookup"><span data-stu-id="f9ce0-124">originSystem</span></span>|<span data-ttu-id="f9ce0-125">String</span><span class="sxs-lookup"><span data-stu-id="f9ce0-125">String</span></span>|<span data-ttu-id="f9ce0-126">O sistema de origem para o escopo.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-126">The origin system for the scope.</span></span>|
|<span data-ttu-id="f9ce0-127">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="f9ce0-127">roleOriginId</span></span>|<span data-ttu-id="f9ce0-128">String</span><span class="sxs-lookup"><span data-stu-id="f9ce0-128">String</span></span>|<span data-ttu-id="f9ce0-129">O sistema de origem para a função, se for diferente.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-129">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="f9ce0-130">url</span><span class="sxs-lookup"><span data-stu-id="f9ce0-130">url</span></span>|<span data-ttu-id="f9ce0-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9ce0-131">String</span></span>|<span data-ttu-id="f9ce0-132">Um localizador de recursos para o escopo.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-132">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9ce0-133">Relações</span><span class="sxs-lookup"><span data-stu-id="f9ce0-133">Relationships</span></span>

| <span data-ttu-id="f9ce0-134">Relação</span><span class="sxs-lookup"><span data-stu-id="f9ce0-134">Relationship</span></span> | <span data-ttu-id="f9ce0-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9ce0-135">Type</span></span>        | <span data-ttu-id="f9ce0-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9ce0-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f9ce0-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="f9ce0-137">accessPackageResource</span></span>|[<span data-ttu-id="f9ce0-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="f9ce0-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="f9ce0-p101">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9ce0-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9ce0-141">JSON representation</span></span>

<span data-ttu-id="f9ce0-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9ce0-142">The following is a JSON representation of the resource.</span></span>

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
