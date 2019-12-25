---
title: tipo de recurso accessPackageResourceScope
description: No gerenciamento de qualificação do Azure AD, um escopo de recurso de pacote do Access é uma referência a um escopo dentro de um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1418e2cb21a1023e864d842b760006e05f3afb03
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870959"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="42cec-103">tipo de recurso accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="42cec-103">accessPackageResourceScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42cec-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um escopo de recurso de pacote do Access é uma referência a um escopo dentro de um recurso, para aqueles recursos que têm vários escopos.</span><span class="sxs-lookup"><span data-stu-id="42cec-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="42cec-105">Você pode determinar o escopo de recurso do pacote de acesso para um recurso que já tenha sido adicionado a um pacote do Access, usando [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) para retornar uma coleção de objetos [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="42cec-105">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="42cec-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42cec-106">Properties</span></span>

| <span data-ttu-id="42cec-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42cec-107">Property</span></span>     | <span data-ttu-id="42cec-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="42cec-108">Type</span></span>        | <span data-ttu-id="42cec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="42cec-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42cec-110">description</span><span class="sxs-lookup"><span data-stu-id="42cec-110">description</span></span>|<span data-ttu-id="42cec-111">String</span><span class="sxs-lookup"><span data-stu-id="42cec-111">String</span></span>|<span data-ttu-id="42cec-112">A descrição do escopo.</span><span class="sxs-lookup"><span data-stu-id="42cec-112">The description of the scope.</span></span>|
|<span data-ttu-id="42cec-113">displayName</span><span class="sxs-lookup"><span data-stu-id="42cec-113">displayName</span></span>|<span data-ttu-id="42cec-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42cec-114">String</span></span>|<span data-ttu-id="42cec-115">O nome de exibição do escopo.</span><span class="sxs-lookup"><span data-stu-id="42cec-115">The display name of the scope.</span></span>|
|<span data-ttu-id="42cec-116">id</span><span class="sxs-lookup"><span data-stu-id="42cec-116">id</span></span>|<span data-ttu-id="42cec-117">String</span><span class="sxs-lookup"><span data-stu-id="42cec-117">String</span></span>| <span data-ttu-id="42cec-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42cec-118">Read-only.</span></span>|
|<span data-ttu-id="42cec-119">isRootScope</span><span class="sxs-lookup"><span data-stu-id="42cec-119">isRootScope</span></span>|<span data-ttu-id="42cec-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="42cec-120">Boolean</span></span>|<span data-ttu-id="42cec-121">True se os escopos são organizados em uma hierarquia e este é o escopo superior ou raiz do recurso.</span><span class="sxs-lookup"><span data-stu-id="42cec-121">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="42cec-122">originid</span><span class="sxs-lookup"><span data-stu-id="42cec-122">originId</span></span>|<span data-ttu-id="42cec-123">String</span><span class="sxs-lookup"><span data-stu-id="42cec-123">String</span></span>|<span data-ttu-id="42cec-124">O identificador exclusivo do escopo no recurso, conforme definido no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="42cec-124">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="42cec-125">originSystem</span><span class="sxs-lookup"><span data-stu-id="42cec-125">originSystem</span></span>|<span data-ttu-id="42cec-126">String</span><span class="sxs-lookup"><span data-stu-id="42cec-126">String</span></span>|<span data-ttu-id="42cec-127">O sistema de origem para o escopo.</span><span class="sxs-lookup"><span data-stu-id="42cec-127">The origin system for the scope.</span></span>|
|<span data-ttu-id="42cec-128">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="42cec-128">roleOriginId</span></span>|<span data-ttu-id="42cec-129">String</span><span class="sxs-lookup"><span data-stu-id="42cec-129">String</span></span>|<span data-ttu-id="42cec-130">O sistema de origem para a função, se for diferente.</span><span class="sxs-lookup"><span data-stu-id="42cec-130">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="42cec-131">url</span><span class="sxs-lookup"><span data-stu-id="42cec-131">url</span></span>|<span data-ttu-id="42cec-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42cec-132">String</span></span>|<span data-ttu-id="42cec-133">Um localizador de recursos para o escopo.</span><span class="sxs-lookup"><span data-stu-id="42cec-133">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42cec-134">Relações</span><span class="sxs-lookup"><span data-stu-id="42cec-134">Relationships</span></span>

| <span data-ttu-id="42cec-135">Relação</span><span class="sxs-lookup"><span data-stu-id="42cec-135">Relationship</span></span> | <span data-ttu-id="42cec-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="42cec-136">Type</span></span>        | <span data-ttu-id="42cec-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="42cec-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42cec-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="42cec-138">accessPackageResource</span></span>|[<span data-ttu-id="42cec-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="42cec-139">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="42cec-p101">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="42cec-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42cec-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42cec-142">JSON representation</span></span>

<span data-ttu-id="42cec-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42cec-143">The following is a JSON representation of the resource.</span></span>

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
