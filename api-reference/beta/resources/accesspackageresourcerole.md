---
title: Tipo de recurso accessPackageResourceRole
description: Uma referência a uma função definida em um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1d7f97410c924b804ef4002932ca75182a461989
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133599"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="2e16d-103">Tipo de recurso accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="2e16d-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="2e16d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e16d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e16d-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma função de recurso do pacote de acesso é uma referência a uma função definida em um recurso.</span><span class="sxs-lookup"><span data-stu-id="2e16d-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="2e16d-106">Essa referência pode ser usada após a criação de um pacote de acesso para especificar as funções de cada um dos recursos do catálogo nos quais um pacote de acesso deve ser entregue, criando um escopo de função de recurso do pacote de [acesso.](../api/accesspackage-post-accesspackageresourcerolescopes.md)</span><span class="sxs-lookup"><span data-stu-id="2e16d-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2e16d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e16d-107">Methods</span></span>

| <span data-ttu-id="2e16d-108">Método</span><span class="sxs-lookup"><span data-stu-id="2e16d-108">Method</span></span>       | <span data-ttu-id="2e16d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e16d-109">Return Type</span></span> | <span data-ttu-id="2e16d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e16d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2e16d-111">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2e16d-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="2e16d-112">[Coleção accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="2e16d-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="2e16d-113">Recupere uma lista de objetos accessPackageResourceRole para um catálogo.</span><span class="sxs-lookup"><span data-stu-id="2e16d-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="2e16d-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e16d-114">Properties</span></span>

| <span data-ttu-id="2e16d-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e16d-115">Property</span></span>     | <span data-ttu-id="2e16d-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e16d-116">Type</span></span>        | <span data-ttu-id="2e16d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e16d-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e16d-118">description</span><span class="sxs-lookup"><span data-stu-id="2e16d-118">description</span></span>|<span data-ttu-id="2e16d-119">String</span><span class="sxs-lookup"><span data-stu-id="2e16d-119">String</span></span>|<span data-ttu-id="2e16d-120">Uma descrição para a função de recurso.</span><span class="sxs-lookup"><span data-stu-id="2e16d-120">A description for the resource role.</span></span>|
|<span data-ttu-id="2e16d-121">displayName</span><span class="sxs-lookup"><span data-stu-id="2e16d-121">displayName</span></span>|<span data-ttu-id="2e16d-122">String</span><span class="sxs-lookup"><span data-stu-id="2e16d-122">String</span></span>|<span data-ttu-id="2e16d-123">O nome de exibição da função de recurso, como a função definida pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2e16d-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="2e16d-124">id</span><span class="sxs-lookup"><span data-stu-id="2e16d-124">id</span></span>|<span data-ttu-id="2e16d-125">String</span><span class="sxs-lookup"><span data-stu-id="2e16d-125">String</span></span>| <span data-ttu-id="2e16d-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e16d-126">Read-only.</span></span>|
|<span data-ttu-id="2e16d-127">originId</span><span class="sxs-lookup"><span data-stu-id="2e16d-127">originId</span></span>|<span data-ttu-id="2e16d-128">String</span><span class="sxs-lookup"><span data-stu-id="2e16d-128">String</span></span>|<span data-ttu-id="2e16d-129">O identificador exclusivo da função de recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="2e16d-129">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="2e16d-130">originSystem</span><span class="sxs-lookup"><span data-stu-id="2e16d-130">originSystem</span></span>|<span data-ttu-id="2e16d-131">String</span><span class="sxs-lookup"><span data-stu-id="2e16d-131">String</span></span>|<span data-ttu-id="2e16d-132">O tipo do recurso no sistema de origem, `SharePointOnline` como, `AadApplication` ou `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="2e16d-132">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e16d-133">Relações</span><span class="sxs-lookup"><span data-stu-id="2e16d-133">Relationships</span></span>

| <span data-ttu-id="2e16d-134">Relação</span><span class="sxs-lookup"><span data-stu-id="2e16d-134">Relationship</span></span> | <span data-ttu-id="2e16d-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e16d-135">Type</span></span>        | <span data-ttu-id="2e16d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e16d-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e16d-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="2e16d-137">accessPackageResource</span></span>|[<span data-ttu-id="2e16d-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="2e16d-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="2e16d-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2e16d-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e16d-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e16d-141">JSON representation</span></span>

<span data-ttu-id="2e16d-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e16d-142">The following is a JSON representation of the resource.</span></span>

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


