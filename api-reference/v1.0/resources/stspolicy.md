---
title: tipo de recurso stsPolicy
description: Representa um tipo de base abstrato para tipos de política que controlam o comportamento da plataforma de identidade da Microsoft.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb43f538fe961af85c1a92f5e853ae8bca44b418
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581901"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="47968-103">tipo de recurso stsPolicy</span><span class="sxs-lookup"><span data-stu-id="47968-103">stsPolicy resource type</span></span>

<span data-ttu-id="47968-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47968-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47968-105">Representa um tipo de base abstrato para tipos de política que controlam o comportamento da [plataforma de identidade da Microsoft](/azure/active-directory/develop/) .</span><span class="sxs-lookup"><span data-stu-id="47968-105">Represents an abstract base type for policy types that control [Microsoft identity platform](/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="47968-106">Herda de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="47968-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="47968-107">Methods</span><span class="sxs-lookup"><span data-stu-id="47968-107">Methods</span></span>

<span data-ttu-id="47968-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47968-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="47968-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47968-109">Properties</span></span>

| <span data-ttu-id="47968-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47968-110">Property</span></span>     | <span data-ttu-id="47968-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="47968-111">Type</span></span>        | <span data-ttu-id="47968-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="47968-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="47968-113">id</span><span class="sxs-lookup"><span data-stu-id="47968-113">id</span></span>|<span data-ttu-id="47968-114">String</span><span class="sxs-lookup"><span data-stu-id="47968-114">String</span></span>| <span data-ttu-id="47968-115">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="47968-115">Unique identifier for this policy.</span></span> <span data-ttu-id="47968-116">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="47968-116">Read-only.</span></span> <span data-ttu-id="47968-117">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="47968-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="47968-118">description</span><span class="sxs-lookup"><span data-stu-id="47968-118">description</span></span>|<span data-ttu-id="47968-119">String</span><span class="sxs-lookup"><span data-stu-id="47968-119">String</span></span>| <span data-ttu-id="47968-120">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="47968-120">Description for this policy.</span></span> <span data-ttu-id="47968-121">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="47968-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="47968-122">displayName</span><span class="sxs-lookup"><span data-stu-id="47968-122">displayName</span></span>|<span data-ttu-id="47968-123">String</span><span class="sxs-lookup"><span data-stu-id="47968-123">String</span></span>| <span data-ttu-id="47968-124">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="47968-124">Display name for this policy.</span></span> <span data-ttu-id="47968-125">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="47968-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="47968-126">definir</span><span class="sxs-lookup"><span data-stu-id="47968-126">definition</span></span>|<span data-ttu-id="47968-127">String collection</span><span class="sxs-lookup"><span data-stu-id="47968-127">String collection</span></span>| <span data-ttu-id="47968-128">Uma coleção String contendo uma cadeia de caracteres JSON que define as regras e configurações de uma política.</span><span class="sxs-lookup"><span data-stu-id="47968-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="47968-129">A sintaxe da definição difere para cada tipo de política derivada.</span><span class="sxs-lookup"><span data-stu-id="47968-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="47968-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47968-130">Required.</span></span>|
|<span data-ttu-id="47968-131">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="47968-131">isOrganizationDefault</span></span>|<span data-ttu-id="47968-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="47968-132">Boolean</span></span>|<span data-ttu-id="47968-133">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="47968-133">If set to true, activates this policy.</span></span> <span data-ttu-id="47968-134">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="47968-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="47968-135">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="47968-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47968-136">Relações</span><span class="sxs-lookup"><span data-stu-id="47968-136">Relationships</span></span>

<span data-ttu-id="47968-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47968-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47968-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47968-138">JSON representation</span></span>

<span data-ttu-id="47968-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47968-139">The following is a JSON representation of the resource.</span></span>

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