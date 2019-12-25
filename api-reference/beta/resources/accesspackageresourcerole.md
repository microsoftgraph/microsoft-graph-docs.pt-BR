---
title: tipo de recurso accessPackageResourceRole
description: Uma referência a uma função definida em um Resource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 21cda352cb887a377248a3fbbf16a761773128ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870419"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="9ac17-103">tipo de recurso accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="9ac17-103">accessPackageResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ac17-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de pacote do Access é uma referência a uma função definida em um recurso, que pode ser usada em um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="9ac17-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="methods"></a><span data-ttu-id="9ac17-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9ac17-105">Methods</span></span>

| <span data-ttu-id="9ac17-106">Método</span><span class="sxs-lookup"><span data-stu-id="9ac17-106">Method</span></span>       | <span data-ttu-id="9ac17-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9ac17-107">Return Type</span></span> | <span data-ttu-id="9ac17-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ac17-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9ac17-109">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="9ac17-109">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="9ac17-110">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="9ac17-110">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="9ac17-111">Recupere uma lista de objetos accessPackageResourceRole para um catálogo.</span><span class="sxs-lookup"><span data-stu-id="9ac17-111">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="9ac17-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ac17-112">Properties</span></span>

| <span data-ttu-id="9ac17-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ac17-113">Property</span></span>     | <span data-ttu-id="9ac17-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ac17-114">Type</span></span>        | <span data-ttu-id="9ac17-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ac17-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9ac17-116">description</span><span class="sxs-lookup"><span data-stu-id="9ac17-116">description</span></span>|<span data-ttu-id="9ac17-117">String</span><span class="sxs-lookup"><span data-stu-id="9ac17-117">String</span></span>|<span data-ttu-id="9ac17-118">Uma descrição para a função de recurso.</span><span class="sxs-lookup"><span data-stu-id="9ac17-118">A description for the resource role.</span></span>|
|<span data-ttu-id="9ac17-119">displayName</span><span class="sxs-lookup"><span data-stu-id="9ac17-119">displayName</span></span>|<span data-ttu-id="9ac17-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac17-120">String</span></span>|<span data-ttu-id="9ac17-121">O nome de exibição da função de recurso como a função definida pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ac17-121">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="9ac17-122">id</span><span class="sxs-lookup"><span data-stu-id="9ac17-122">id</span></span>|<span data-ttu-id="9ac17-123">String</span><span class="sxs-lookup"><span data-stu-id="9ac17-123">String</span></span>| <span data-ttu-id="9ac17-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ac17-124">Read-only.</span></span>|
|<span data-ttu-id="9ac17-125">originid</span><span class="sxs-lookup"><span data-stu-id="9ac17-125">originId</span></span>|<span data-ttu-id="9ac17-126">String</span><span class="sxs-lookup"><span data-stu-id="9ac17-126">String</span></span>|<span data-ttu-id="9ac17-127">O identificador exclusivo da função de recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="9ac17-127">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="9ac17-128">originSystem</span><span class="sxs-lookup"><span data-stu-id="9ac17-128">originSystem</span></span>|<span data-ttu-id="9ac17-129">String</span><span class="sxs-lookup"><span data-stu-id="9ac17-129">String</span></span>|<span data-ttu-id="9ac17-130">O tipo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="9ac17-130">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ac17-131">Relações</span><span class="sxs-lookup"><span data-stu-id="9ac17-131">Relationships</span></span>

| <span data-ttu-id="9ac17-132">Relação</span><span class="sxs-lookup"><span data-stu-id="9ac17-132">Relationship</span></span> | <span data-ttu-id="9ac17-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ac17-133">Type</span></span>        | <span data-ttu-id="9ac17-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ac17-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9ac17-135">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="9ac17-135">accessPackageResource</span></span>|[<span data-ttu-id="9ac17-136">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="9ac17-136">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="9ac17-p101">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="9ac17-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ac17-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ac17-139">JSON representation</span></span>

<span data-ttu-id="9ac17-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ac17-140">The following is a JSON representation of the resource.</span></span>

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
