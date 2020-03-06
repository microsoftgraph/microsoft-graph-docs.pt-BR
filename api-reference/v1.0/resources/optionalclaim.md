---
title: tipo de recurso optionalClaim
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: sureshja
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: de97333a2a7580e9b6a9b58e042c0c5a8ff9bbe7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534125"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="19637-103">tipo de recurso optionalClaim</span><span class="sxs-lookup"><span data-stu-id="19637-103">optionalClaim resource type</span></span>

<span data-ttu-id="19637-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19637-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19637-105">Contém uma declaração opcional associada a um [aplicativo](application.md)</span><span class="sxs-lookup"><span data-stu-id="19637-105">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="19637-106">.</span><span class="sxs-lookup"><span data-stu-id="19637-106">.</span></span> <span data-ttu-id="19637-107">As `idToken`propriedades `accessToken`,, `saml2Token` e do recurso [optionalClaims](optionalclaims.md) é uma coleção de **optionalClaim**.</span><span class="sxs-lookup"><span data-stu-id="19637-107">The `idToken`, `accessToken`, and `saml2Token` properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="19637-108">Se houver suporte para uma declaração específica, você também poderá modificar o comportamento do optionalClaim usando a `additionalProperties` propriedade.</span><span class="sxs-lookup"><span data-stu-id="19637-108">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span>

<span data-ttu-id="19637-109">Confira [fornecer declarações opcionais ao aplicativo Azure AD](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="19637-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="19637-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19637-110">Properties</span></span>

| <span data-ttu-id="19637-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19637-111">Property</span></span>     | <span data-ttu-id="19637-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="19637-112">Type</span></span>        | <span data-ttu-id="19637-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="19637-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19637-114">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="19637-114">additionalProperties</span></span>|<span data-ttu-id="19637-115">String collection</span><span class="sxs-lookup"><span data-stu-id="19637-115">String collection</span></span>| <span data-ttu-id="19637-116">Propriedades adicionais da declaração.</span><span class="sxs-lookup"><span data-stu-id="19637-116">Additional properties of the claim.</span></span> <span data-ttu-id="19637-117">Se uma propriedade existir nessa coleção, ela modificará o comportamento da declaração opcional especificada na propriedade Name.</span><span class="sxs-lookup"><span data-stu-id="19637-117">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="19637-118">essencial</span><span class="sxs-lookup"><span data-stu-id="19637-118">essential</span></span>|<span data-ttu-id="19637-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="19637-119">Boolean</span></span>| <span data-ttu-id="19637-120">Se o valor for true, a declaração especificada pelo cliente será necessária para garantir uma experiência de autorização suave para a tarefa específica solicitada pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="19637-120">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="19637-121">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="19637-121">The default value is false.</span></span>|
|<span data-ttu-id="19637-122">nome</span><span class="sxs-lookup"><span data-stu-id="19637-122">name</span></span>|<span data-ttu-id="19637-123">String</span><span class="sxs-lookup"><span data-stu-id="19637-123">String</span></span>| <span data-ttu-id="19637-124">O nome da declaração opcional.</span><span class="sxs-lookup"><span data-stu-id="19637-124">The name of the optional claim.</span></span> |
|<span data-ttu-id="19637-125">source</span><span class="sxs-lookup"><span data-stu-id="19637-125">source</span></span>|<span data-ttu-id="19637-126">String</span><span class="sxs-lookup"><span data-stu-id="19637-126">String</span></span>| <span data-ttu-id="19637-127">A origem (objeto de diretório) da declaração.</span><span class="sxs-lookup"><span data-stu-id="19637-127">The source (directory object) of the claim.</span></span> <span data-ttu-id="19637-128">Há declarações predefinidas e declarações definidas pelo usuário das propriedades de extensão.</span><span class="sxs-lookup"><span data-stu-id="19637-128">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="19637-129">Se o valor de origem for nulo, a declaração será uma declaração opcional predefinida.</span><span class="sxs-lookup"><span data-stu-id="19637-129">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="19637-130">Se o valor de origem for User, o valor na propriedade Name será a Propriedade Extension do objeto user.</span><span class="sxs-lookup"><span data-stu-id="19637-130">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="19637-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19637-131">JSON representation</span></span>

<span data-ttu-id="19637-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19637-132">The following is a JSON representation of the resource.</span></span>

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