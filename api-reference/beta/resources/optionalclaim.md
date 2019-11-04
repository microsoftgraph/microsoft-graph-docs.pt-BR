---
title: tipo de recurso optionalClaim
description: Contém uma declaração opcional associada a um aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a62176c1e662b1d292f6f359cb2021fae684f4ee
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935040"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="3c2a6-103">tipo de recurso optionalClaim</span><span class="sxs-lookup"><span data-stu-id="3c2a6-103">optionalClaim resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c2a6-104">Contém uma declaração opcional associada a um [aplicativo](application.md)</span><span class="sxs-lookup"><span data-stu-id="3c2a6-104">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="3c2a6-105">.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-105"></span></span> <span data-ttu-id="3c2a6-106">As propriedades **idToken**, **accessToken**e **saml2Token** do recurso [optionalClaims](optionalclaims.md) é uma coleção de **optionalClaim**.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-106">The **idToken**, **accessToken**, and **saml2Token** properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="3c2a6-107">Se houver suporte para uma declaração específica, você também poderá modificar o comportamento do optionalClaim usando a `additionalProperties` propriedade.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-107">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span> 

<span data-ttu-id="3c2a6-108">Consulte [fornecer declarações opcionais para seu aplicativo do Azure ad](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-108">See [provide optional claims to your Azure AD app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="3c2a6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c2a6-109">Properties</span></span>

| <span data-ttu-id="3c2a6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c2a6-110">Property</span></span>     | <span data-ttu-id="3c2a6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c2a6-111">Type</span></span>        | <span data-ttu-id="3c2a6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c2a6-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3c2a6-113">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="3c2a6-113">additionalProperties</span></span>|<span data-ttu-id="3c2a6-114">String collection</span><span class="sxs-lookup"><span data-stu-id="3c2a6-114">String collection</span></span>| <span data-ttu-id="3c2a6-115">Propriedades adicionais da declaração.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-115">Additional properties of the claim.</span></span> <span data-ttu-id="3c2a6-116">Se uma propriedade existir nessa coleção, ela modificará o comportamento da declaração opcional especificada na propriedade Name.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-116">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="3c2a6-117">essencial</span><span class="sxs-lookup"><span data-stu-id="3c2a6-117">essential</span></span>|<span data-ttu-id="3c2a6-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="3c2a6-118">Boolean</span></span>| <span data-ttu-id="3c2a6-119">Se o valor for true, a declaração especificada pelo cliente será necessária para garantir uma experiência de autorização suave para a tarefa específica solicitada pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-119">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="3c2a6-120">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-120">The default value is false.</span></span>|
|<span data-ttu-id="3c2a6-121">name</span><span class="sxs-lookup"><span data-stu-id="3c2a6-121">name</span></span>|<span data-ttu-id="3c2a6-122">String</span><span class="sxs-lookup"><span data-stu-id="3c2a6-122">String</span></span>| <span data-ttu-id="3c2a6-123">O nome da declaração opcional.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-123">The name of the optional claim.</span></span> |
|<span data-ttu-id="3c2a6-124">source</span><span class="sxs-lookup"><span data-stu-id="3c2a6-124">source</span></span>|<span data-ttu-id="3c2a6-125">String</span><span class="sxs-lookup"><span data-stu-id="3c2a6-125">String</span></span>| <span data-ttu-id="3c2a6-126">A origem (objeto de diretório) da declaração.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-126">The source (directory object) of the claim.</span></span> <span data-ttu-id="3c2a6-127">Há declarações predefinidas e declarações definidas pelo usuário das propriedades de extensão.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-127">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="3c2a6-128">Se o valor de origem for nulo, a declaração será uma declaração opcional predefinida.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-128">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="3c2a6-129">Se o valor de origem for User, o valor na propriedade Name será a Propriedade Extension do objeto user.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-129">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3c2a6-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c2a6-130">JSON representation</span></span>

<span data-ttu-id="3c2a6-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c2a6-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.optionalClaim",
  "baseType": null
}-->

```json
{
  "additionalProperties": ["String"],
  "essential": true,
  "name": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "optionalClaim resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
