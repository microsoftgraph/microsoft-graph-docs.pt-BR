---
title: tipo de recurso accessPackageResourceRole
description: Uma referência a uma função definida em um Resource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b5ae5d321ac5fec86801ca11f60ead8a276fd73
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938916"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="36e3a-103">tipo de recurso accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="36e3a-103">accessPackageResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36e3a-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de pacote do Access é uma referência a uma função definida em um recurso, que pode ser usada em um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="36e3a-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="36e3a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36e3a-105">Properties</span></span>

| <span data-ttu-id="36e3a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36e3a-106">Property</span></span>     | <span data-ttu-id="36e3a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="36e3a-107">Type</span></span>        | <span data-ttu-id="36e3a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="36e3a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36e3a-109">description</span><span class="sxs-lookup"><span data-stu-id="36e3a-109">description</span></span>|<span data-ttu-id="36e3a-110">String</span><span class="sxs-lookup"><span data-stu-id="36e3a-110">String</span></span>|<span data-ttu-id="36e3a-111">Uma descrição para a função de recurso.</span><span class="sxs-lookup"><span data-stu-id="36e3a-111">A description for the resource role.</span></span>|
|<span data-ttu-id="36e3a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="36e3a-112">displayName</span></span>|<span data-ttu-id="36e3a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36e3a-113">String</span></span>|<span data-ttu-id="36e3a-114">O nome de exibição da função de recurso como a função definida pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="36e3a-114">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="36e3a-115">id</span><span class="sxs-lookup"><span data-stu-id="36e3a-115">id</span></span>|<span data-ttu-id="36e3a-116">String</span><span class="sxs-lookup"><span data-stu-id="36e3a-116">String</span></span>| <span data-ttu-id="36e3a-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36e3a-117">Read-only.</span></span>|
|<span data-ttu-id="36e3a-118">originid</span><span class="sxs-lookup"><span data-stu-id="36e3a-118">originId</span></span>|<span data-ttu-id="36e3a-119">String</span><span class="sxs-lookup"><span data-stu-id="36e3a-119">String</span></span>|<span data-ttu-id="36e3a-120">O identificador exclusivo da função de recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="36e3a-120">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="36e3a-121">originSystem</span><span class="sxs-lookup"><span data-stu-id="36e3a-121">originSystem</span></span>|<span data-ttu-id="36e3a-122">String</span><span class="sxs-lookup"><span data-stu-id="36e3a-122">String</span></span>|<span data-ttu-id="36e3a-123">O tipo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="36e3a-123">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36e3a-124">Relações</span><span class="sxs-lookup"><span data-stu-id="36e3a-124">Relationships</span></span>

| <span data-ttu-id="36e3a-125">Relação</span><span class="sxs-lookup"><span data-stu-id="36e3a-125">Relationship</span></span> | <span data-ttu-id="36e3a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="36e3a-126">Type</span></span>        | <span data-ttu-id="36e3a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="36e3a-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36e3a-128">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="36e3a-128">accessPackageResource</span></span>|[<span data-ttu-id="36e3a-129">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="36e3a-129">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="36e3a-p101">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="36e3a-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36e3a-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36e3a-132">JSON representation</span></span>

<span data-ttu-id="36e3a-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36e3a-133">The following is a JSON representation of the resource.</span></span>

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
