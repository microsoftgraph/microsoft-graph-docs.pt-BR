---
title: Tipo de recurso stsPolicy
description: Representa um tipo de base abstrato para tipos de política que controlam o comportamento da plataforma de identidade da Microsoft.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 362b0ec08cfc7b3fe96b67baf4e8ed4aa2b86495
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761554"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="4b7be-103">Tipo de recurso stsPolicy</span><span class="sxs-lookup"><span data-stu-id="4b7be-103">stsPolicy resource type</span></span>

<span data-ttu-id="4b7be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b7be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b7be-105">Representa um tipo de base abstrato para tipos de política que controlam o [comportamento da plataforma de identidade da Microsoft.](/azure/active-directory/develop/)</span><span class="sxs-lookup"><span data-stu-id="4b7be-105">Represents an abstract base type for policy types that control [Microsoft identity platform](/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="4b7be-106">Herda de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="4b7be-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4b7be-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4b7be-107">Methods</span></span>

<span data-ttu-id="4b7be-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b7be-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="4b7be-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b7be-109">Properties</span></span>

| <span data-ttu-id="4b7be-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b7be-110">Property</span></span>     | <span data-ttu-id="4b7be-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b7be-111">Type</span></span>        | <span data-ttu-id="4b7be-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b7be-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b7be-113">id</span><span class="sxs-lookup"><span data-stu-id="4b7be-113">id</span></span>|<span data-ttu-id="4b7be-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b7be-114">String</span></span>| <span data-ttu-id="4b7be-115">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="4b7be-115">Unique identifier for this policy.</span></span> <span data-ttu-id="4b7be-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4b7be-116">Read-only.</span></span> <span data-ttu-id="4b7be-117">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="4b7be-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="4b7be-118">descrição</span><span class="sxs-lookup"><span data-stu-id="4b7be-118">description</span></span>|<span data-ttu-id="4b7be-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b7be-119">String</span></span>| <span data-ttu-id="4b7be-120">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="4b7be-120">Description for this policy.</span></span> <span data-ttu-id="4b7be-121">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="4b7be-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="4b7be-122">displayName</span><span class="sxs-lookup"><span data-stu-id="4b7be-122">displayName</span></span>|<span data-ttu-id="4b7be-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b7be-123">String</span></span>| <span data-ttu-id="4b7be-124">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="4b7be-124">Display name for this policy.</span></span> <span data-ttu-id="4b7be-125">Herdado de [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="4b7be-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="4b7be-126">definition</span><span class="sxs-lookup"><span data-stu-id="4b7be-126">definition</span></span>|<span data-ttu-id="4b7be-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b7be-127">String collection</span></span>| <span data-ttu-id="4b7be-128">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações de uma política.</span><span class="sxs-lookup"><span data-stu-id="4b7be-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="4b7be-129">A sintaxe da definição difere para cada tipo de política derivado.</span><span class="sxs-lookup"><span data-stu-id="4b7be-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="4b7be-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b7be-130">Required.</span></span>|
|<span data-ttu-id="4b7be-131">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="4b7be-131">isOrganizationDefault</span></span>|<span data-ttu-id="4b7be-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b7be-132">Boolean</span></span>|<span data-ttu-id="4b7be-133">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="4b7be-133">If set to true, activates this policy.</span></span> <span data-ttu-id="4b7be-134">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="4b7be-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="4b7be-135">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="4b7be-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b7be-136">Relações</span><span class="sxs-lookup"><span data-stu-id="4b7be-136">Relationships</span></span>

<span data-ttu-id="4b7be-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b7be-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b7be-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b7be-138">JSON representation</span></span>

<span data-ttu-id="4b7be-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b7be-139">The following is a JSON representation of the resource.</span></span>

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