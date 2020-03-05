---
title: tipo de recurso accessPackageResourceRole
description: Uma referência a uma função definida em um Resource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b5ab0cc6e2179adb62316cbcdc06b7dd52abc439
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508510"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="e7668-103">tipo de recurso accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="e7668-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="e7668-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e7668-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7668-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de pacote do Access é uma referência a uma função definida em um recurso, que pode ser usada em um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="e7668-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="methods"></a><span data-ttu-id="e7668-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e7668-106">Methods</span></span>

| <span data-ttu-id="e7668-107">Método</span><span class="sxs-lookup"><span data-stu-id="e7668-107">Method</span></span>       | <span data-ttu-id="e7668-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e7668-108">Return Type</span></span> | <span data-ttu-id="e7668-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7668-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7668-110">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="e7668-110">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="e7668-111">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="e7668-111">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="e7668-112">Recupere uma lista de objetos accessPackageResourceRole para um catálogo.</span><span class="sxs-lookup"><span data-stu-id="e7668-112">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7668-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7668-113">Properties</span></span>

| <span data-ttu-id="e7668-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7668-114">Property</span></span>     | <span data-ttu-id="e7668-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7668-115">Type</span></span>        | <span data-ttu-id="e7668-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7668-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7668-117">description</span><span class="sxs-lookup"><span data-stu-id="e7668-117">description</span></span>|<span data-ttu-id="e7668-118">String</span><span class="sxs-lookup"><span data-stu-id="e7668-118">String</span></span>|<span data-ttu-id="e7668-119">Uma descrição para a função de recurso.</span><span class="sxs-lookup"><span data-stu-id="e7668-119">A description for the resource role.</span></span>|
|<span data-ttu-id="e7668-120">displayName</span><span class="sxs-lookup"><span data-stu-id="e7668-120">displayName</span></span>|<span data-ttu-id="e7668-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7668-121">String</span></span>|<span data-ttu-id="e7668-122">O nome de exibição da função de recurso como a função definida pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7668-122">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="e7668-123">id</span><span class="sxs-lookup"><span data-stu-id="e7668-123">id</span></span>|<span data-ttu-id="e7668-124">String</span><span class="sxs-lookup"><span data-stu-id="e7668-124">String</span></span>| <span data-ttu-id="e7668-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7668-125">Read-only.</span></span>|
|<span data-ttu-id="e7668-126">originid</span><span class="sxs-lookup"><span data-stu-id="e7668-126">originId</span></span>|<span data-ttu-id="e7668-127">String</span><span class="sxs-lookup"><span data-stu-id="e7668-127">String</span></span>|<span data-ttu-id="e7668-128">O identificador exclusivo da função de recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="e7668-128">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="e7668-129">originSystem</span><span class="sxs-lookup"><span data-stu-id="e7668-129">originSystem</span></span>|<span data-ttu-id="e7668-130">String</span><span class="sxs-lookup"><span data-stu-id="e7668-130">String</span></span>|<span data-ttu-id="e7668-131">O tipo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="e7668-131">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7668-132">Relações</span><span class="sxs-lookup"><span data-stu-id="e7668-132">Relationships</span></span>

| <span data-ttu-id="e7668-133">Relação</span><span class="sxs-lookup"><span data-stu-id="e7668-133">Relationship</span></span> | <span data-ttu-id="e7668-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7668-134">Type</span></span>        | <span data-ttu-id="e7668-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7668-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7668-136">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e7668-136">accessPackageResource</span></span>|[<span data-ttu-id="e7668-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e7668-137">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="e7668-p101">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e7668-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7668-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7668-140">JSON representation</span></span>

<span data-ttu-id="e7668-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7668-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
