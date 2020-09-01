---
title: tipo de recurso accessPackageResourceRole
description: Uma referência a uma função definida em um Resource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bc0a60043c9877b4c48a889f93fa48a852c3780
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319579"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="57dd0-103">tipo de recurso accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="57dd0-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="57dd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57dd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57dd0-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de pacote do Access é uma referência a uma função definida em um recurso.</span><span class="sxs-lookup"><span data-stu-id="57dd0-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="57dd0-106">Essa referência pode ser usada após a criação de um pacote do Access para especificar as funções de cada um dos recursos do catálogo nos quais um pacote do Access deve fornecer, [criando um escopo de função de recurso de pacote do Access](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span><span class="sxs-lookup"><span data-stu-id="57dd0-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="57dd0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="57dd0-107">Methods</span></span>

| <span data-ttu-id="57dd0-108">Método</span><span class="sxs-lookup"><span data-stu-id="57dd0-108">Method</span></span>       | <span data-ttu-id="57dd0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="57dd0-109">Return Type</span></span> | <span data-ttu-id="57dd0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="57dd0-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="57dd0-111">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="57dd0-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="57dd0-112">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="57dd0-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="57dd0-113">Recupere uma lista de objetos accessPackageResourceRole para um catálogo.</span><span class="sxs-lookup"><span data-stu-id="57dd0-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="57dd0-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57dd0-114">Properties</span></span>

| <span data-ttu-id="57dd0-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57dd0-115">Property</span></span>     | <span data-ttu-id="57dd0-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="57dd0-116">Type</span></span>        | <span data-ttu-id="57dd0-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="57dd0-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="57dd0-118">description</span><span class="sxs-lookup"><span data-stu-id="57dd0-118">description</span></span>|<span data-ttu-id="57dd0-119">String</span><span class="sxs-lookup"><span data-stu-id="57dd0-119">String</span></span>|<span data-ttu-id="57dd0-120">Uma descrição para a função de recurso.</span><span class="sxs-lookup"><span data-stu-id="57dd0-120">A description for the resource role.</span></span>|
|<span data-ttu-id="57dd0-121">displayName</span><span class="sxs-lookup"><span data-stu-id="57dd0-121">displayName</span></span>|<span data-ttu-id="57dd0-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57dd0-122">String</span></span>|<span data-ttu-id="57dd0-123">O nome de exibição da função de recurso como a função definida pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57dd0-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="57dd0-124">id</span><span class="sxs-lookup"><span data-stu-id="57dd0-124">id</span></span>|<span data-ttu-id="57dd0-125">String</span><span class="sxs-lookup"><span data-stu-id="57dd0-125">String</span></span>| <span data-ttu-id="57dd0-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="57dd0-126">Read-only.</span></span>|
|<span data-ttu-id="57dd0-127">originid</span><span class="sxs-lookup"><span data-stu-id="57dd0-127">originId</span></span>|<span data-ttu-id="57dd0-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57dd0-128">String</span></span>|<span data-ttu-id="57dd0-129">O identificador exclusivo da função de recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="57dd0-129">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="57dd0-130">originSystem</span><span class="sxs-lookup"><span data-stu-id="57dd0-130">originSystem</span></span>|<span data-ttu-id="57dd0-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57dd0-131">String</span></span>|<span data-ttu-id="57dd0-132">O tipo do recurso no sistema de origem, como `SharePointOnline` , `AadApplication` ou `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="57dd0-132">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57dd0-133">Relações</span><span class="sxs-lookup"><span data-stu-id="57dd0-133">Relationships</span></span>

| <span data-ttu-id="57dd0-134">Relação</span><span class="sxs-lookup"><span data-stu-id="57dd0-134">Relationship</span></span> | <span data-ttu-id="57dd0-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="57dd0-135">Type</span></span>        | <span data-ttu-id="57dd0-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="57dd0-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="57dd0-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="57dd0-137">accessPackageResource</span></span>|[<span data-ttu-id="57dd0-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="57dd0-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="57dd0-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="57dd0-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57dd0-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57dd0-141">JSON representation</span></span>

<span data-ttu-id="57dd0-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57dd0-142">The following is a JSON representation of the resource.</span></span>

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
