---
title: tipo de recurso stsPolicy
description: Representa um tipo de base abstrato para tipos de política que controlam o comportamento da plataforma de identidade da Microsoft.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56032480861e52190c9ea2dd80da82c70068c429
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917520"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="e8b28-103">tipo de recurso stsPolicy</span><span class="sxs-lookup"><span data-stu-id="e8b28-103">stsPolicy resource type</span></span>

<span data-ttu-id="e8b28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8b28-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8b28-105">Representa um tipo de base abstrato para tipos de política que controlam o comportamento da [plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/) .</span><span class="sxs-lookup"><span data-stu-id="e8b28-105">Represents an abstract base type for policy types that control [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="e8b28-106">Herda de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="e8b28-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e8b28-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e8b28-107">Methods</span></span>

<span data-ttu-id="e8b28-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8b28-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="e8b28-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8b28-109">Properties</span></span>

| <span data-ttu-id="e8b28-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8b28-110">Property</span></span>     | <span data-ttu-id="e8b28-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8b28-111">Type</span></span>        | <span data-ttu-id="e8b28-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8b28-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8b28-113">id</span><span class="sxs-lookup"><span data-stu-id="e8b28-113">id</span></span>|<span data-ttu-id="e8b28-114">String</span><span class="sxs-lookup"><span data-stu-id="e8b28-114">String</span></span>| <span data-ttu-id="e8b28-115">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="e8b28-115">Unique identifier for this policy.</span></span> <span data-ttu-id="e8b28-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8b28-116">Read-only.</span></span> <span data-ttu-id="e8b28-117">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="e8b28-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="e8b28-118">description</span><span class="sxs-lookup"><span data-stu-id="e8b28-118">description</span></span>|<span data-ttu-id="e8b28-119">String</span><span class="sxs-lookup"><span data-stu-id="e8b28-119">String</span></span>| <span data-ttu-id="e8b28-120">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="e8b28-120">Description for this policy.</span></span> <span data-ttu-id="e8b28-121">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="e8b28-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="e8b28-122">displayName</span><span class="sxs-lookup"><span data-stu-id="e8b28-122">displayName</span></span>|<span data-ttu-id="e8b28-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8b28-123">String</span></span>| <span data-ttu-id="e8b28-124">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="e8b28-124">Display name for this policy.</span></span> <span data-ttu-id="e8b28-125">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="e8b28-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="e8b28-126">definir</span><span class="sxs-lookup"><span data-stu-id="e8b28-126">definition</span></span>|<span data-ttu-id="e8b28-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8b28-127">String collection</span></span>| <span data-ttu-id="e8b28-128">Uma coleção String contendo uma cadeia de caracteres JSON que define as regras e configurações de uma política.</span><span class="sxs-lookup"><span data-stu-id="e8b28-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="e8b28-129">A sintaxe da definição difere para cada tipo de política derivada.</span><span class="sxs-lookup"><span data-stu-id="e8b28-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="e8b28-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8b28-130">Required.</span></span>|
|<span data-ttu-id="e8b28-131">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="e8b28-131">isOrganizationDefault</span></span>|<span data-ttu-id="e8b28-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8b28-132">Boolean</span></span>|<span data-ttu-id="e8b28-133">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="e8b28-133">If set to true, activates this policy.</span></span> <span data-ttu-id="e8b28-134">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="e8b28-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="e8b28-135">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="e8b28-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8b28-136">Relações</span><span class="sxs-lookup"><span data-stu-id="e8b28-136">Relationships</span></span>

<span data-ttu-id="e8b28-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8b28-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8b28-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8b28-138">JSON representation</span></span>

<span data-ttu-id="e8b28-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8b28-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stsPolicy",
  "baseType": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": ["String"],
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
