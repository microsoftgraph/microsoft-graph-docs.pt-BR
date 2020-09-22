---
title: tipo de recurso ACL
description: Uma entrada de controle de acesso para um item indexado por um externalConnection de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6d390ac0fee3063bd8f0d292d14e04b2616c1d00
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193530"
---
# <a name="acl-resource-type"></a><span data-ttu-id="56c01-103">tipo de recurso ACL</span><span class="sxs-lookup"><span data-stu-id="56c01-103">acl resource type</span></span>

<span data-ttu-id="56c01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56c01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56c01-105">Uma entrada de controle de acesso para um item indexado por um [externalConnection](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="56c01-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="56c01-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56c01-106">Properties</span></span>

| <span data-ttu-id="56c01-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56c01-107">Property</span></span>       | <span data-ttu-id="56c01-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="56c01-108">Type</span></span>   | <span data-ttu-id="56c01-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="56c01-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="56c01-110">accessType</span><span class="sxs-lookup"><span data-stu-id="56c01-110">accessType</span></span>     | <span data-ttu-id="56c01-111">String</span><span class="sxs-lookup"><span data-stu-id="56c01-111">String</span></span> | <span data-ttu-id="56c01-112">O acesso concedido à identidade.</span><span class="sxs-lookup"><span data-stu-id="56c01-112">The access granted to the identity.</span></span> <span data-ttu-id="56c01-113">Os valores possíveis são: `grant` e `deny`.</span><span class="sxs-lookup"><span data-stu-id="56c01-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="56c01-114">identificação da identidade</span><span class="sxs-lookup"><span data-stu-id="56c01-114">identitySource</span></span> | <span data-ttu-id="56c01-115">String</span><span class="sxs-lookup"><span data-stu-id="56c01-115">String</span></span> | <span data-ttu-id="56c01-116">A fonte de identidade.</span><span class="sxs-lookup"><span data-stu-id="56c01-116">The source of identity.</span></span> <span data-ttu-id="56c01-117">Os valores possíveis são `azureActiveDirectory` ou `external` .</span><span class="sxs-lookup"><span data-stu-id="56c01-117">Possible values are `azureActiveDirectory` or `external`.</span></span>           |
| <span data-ttu-id="56c01-118">tipo</span><span class="sxs-lookup"><span data-stu-id="56c01-118">type</span></span>           | <span data-ttu-id="56c01-119">String</span><span class="sxs-lookup"><span data-stu-id="56c01-119">String</span></span> | <span data-ttu-id="56c01-120">O tipo de identidade.</span><span class="sxs-lookup"><span data-stu-id="56c01-120">The type of identity.</span></span> <span data-ttu-id="56c01-121">Os valores possíveis são: `user` , `group` , `everyone` , `everyoneExceptGuests` se a identificação do próprio é `azureActiveDirectory` e apenas `group` se a identificação do próprio é `external` .</span><span class="sxs-lookup"><span data-stu-id="56c01-121">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests` if the identitySource is `azureActiveDirectory` and just `group` if the identitySource is `external`.</span></span> |
| <span data-ttu-id="56c01-122">value</span><span class="sxs-lookup"><span data-stu-id="56c01-122">value</span></span>          | <span data-ttu-id="56c01-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56c01-123">String</span></span> | <span data-ttu-id="56c01-124">O identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="56c01-124">The unique identifer of the identity.</span></span> <span data-ttu-id="56c01-125">No caso de identidades do Active Directory do Azure, `value` é definido como o identificador de objeto do usuário, grupo ou locatário para tipos usuário, grupo e todos (e everyoneExceptGuests), respectivamente.</span><span class="sxs-lookup"><span data-stu-id="56c01-125">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="56c01-126">No caso de grupos externos, `value` está definido como a ID do grupo [externo](externalgroup.md).</span><span class="sxs-lookup"><span data-stu-id="56c01-126">In case of external groups `value` is set to the ID of the [externalGroup](externalgroup.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56c01-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56c01-127">JSON representation</span></span>

<span data-ttu-id="56c01-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56c01-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
