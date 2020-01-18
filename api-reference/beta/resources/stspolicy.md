---
title: tipo de recurso stsPolicy
description: Representa um tipo de base abstrato para tipos de política que controlam o comportamento da plataforma de identidade da Microsoft.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f351d994daba00f4465d934fe570b5db2e704ae9
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234058"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="727d2-103">tipo de recurso policyBase</span><span class="sxs-lookup"><span data-stu-id="727d2-103">policyBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="727d2-104">Representa um tipo de base abstrato para tipos de política que controlam o comportamento da [plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/) .</span><span class="sxs-lookup"><span data-stu-id="727d2-104">Represents an abstract base type for policy types that control [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="727d2-105">Herda de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="727d2-105">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="727d2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="727d2-106">Methods</span></span>

<span data-ttu-id="727d2-107">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="727d2-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="727d2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="727d2-108">Properties</span></span>

| <span data-ttu-id="727d2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="727d2-109">Property</span></span>     | <span data-ttu-id="727d2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="727d2-110">Type</span></span>        | <span data-ttu-id="727d2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="727d2-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="727d2-112">id</span><span class="sxs-lookup"><span data-stu-id="727d2-112">id</span></span>|<span data-ttu-id="727d2-113">String</span><span class="sxs-lookup"><span data-stu-id="727d2-113">String</span></span>| <span data-ttu-id="727d2-114">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="727d2-114">Unique identifier for this policy.</span></span> <span data-ttu-id="727d2-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="727d2-115">Read-only.</span></span> <span data-ttu-id="727d2-116">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="727d2-116">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="727d2-117">description</span><span class="sxs-lookup"><span data-stu-id="727d2-117">description</span></span>|<span data-ttu-id="727d2-118">String</span><span class="sxs-lookup"><span data-stu-id="727d2-118">String</span></span>| <span data-ttu-id="727d2-119">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="727d2-119">Description for this policy.</span></span> <span data-ttu-id="727d2-120">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="727d2-120">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="727d2-121">displayName</span><span class="sxs-lookup"><span data-stu-id="727d2-121">displayName</span></span>|<span data-ttu-id="727d2-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="727d2-122">String</span></span>| <span data-ttu-id="727d2-123">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="727d2-123">Display name for this policy.</span></span> <span data-ttu-id="727d2-124">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="727d2-124">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="727d2-125">definir</span><span class="sxs-lookup"><span data-stu-id="727d2-125">definition</span></span>|<span data-ttu-id="727d2-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="727d2-126">String collection</span></span>| <span data-ttu-id="727d2-127">Uma coleção String contendo uma cadeia de caracteres JSON que define as regras e configurações de uma política.</span><span class="sxs-lookup"><span data-stu-id="727d2-127">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="727d2-128">A sintaxe da definição difere para cada tipo de política derivada.</span><span class="sxs-lookup"><span data-stu-id="727d2-128">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="727d2-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="727d2-129">Required.</span></span>|
|<span data-ttu-id="727d2-130">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="727d2-130">isOrganizationDefault</span></span>|<span data-ttu-id="727d2-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="727d2-131">Boolean</span></span>|<span data-ttu-id="727d2-132">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="727d2-132">If set to true, activates this policy.</span></span> <span data-ttu-id="727d2-133">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="727d2-133">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="727d2-134">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="727d2-134">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="727d2-135">Relações</span><span class="sxs-lookup"><span data-stu-id="727d2-135">Relationships</span></span>

<span data-ttu-id="727d2-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="727d2-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="727d2-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="727d2-137">JSON representation</span></span>

<span data-ttu-id="727d2-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="727d2-138">The following is a JSON representation of the resource.</span></span>

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