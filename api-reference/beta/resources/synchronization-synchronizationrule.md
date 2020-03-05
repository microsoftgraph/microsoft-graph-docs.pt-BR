---
title: tipo de recurso synchronizationRule
description: Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos sincronizar e em que direção, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformada quando estiverem sincronizadas da origem para o diretório de destino.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b1d8afd1f87527a5a92755ff45ec876c8d66d9c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520048"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="2ef67-103">tipo de recurso synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="2ef67-103">synchronizationRule resource type</span></span>

<span data-ttu-id="2ef67-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ef67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef67-105">Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos sincronizar e em que direção, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformada quando estiverem sincronizadas da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="2ef67-105">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="2ef67-106">**Observação:** As regras de sincronização definem a sincronização em uma direção – do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="2ef67-106">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="2ef67-107">Os diretórios de origem e de destino são definidos como parte das propriedades da regra.</span><span class="sxs-lookup"><span data-stu-id="2ef67-107">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="2ef67-108">As regras de sincronização são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2ef67-108">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2ef67-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ef67-109">Properties</span></span>

| <span data-ttu-id="2ef67-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ef67-110">Property</span></span>      | <span data-ttu-id="2ef67-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ef67-111">Type</span></span>      | <span data-ttu-id="2ef67-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef67-112">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="2ef67-113">edita</span><span class="sxs-lookup"><span data-stu-id="2ef67-113">editable</span></span>       |<span data-ttu-id="2ef67-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ef67-114">Boolean</span></span>    |<span data-ttu-id="2ef67-115">`true`se a regra de sincronização puder ser personalizada; `false` se essa regra é somente leitura e não deve ser alterada.</span><span class="sxs-lookup"><span data-stu-id="2ef67-115">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="2ef67-116">id</span><span class="sxs-lookup"><span data-stu-id="2ef67-116">id</span></span>             |<span data-ttu-id="2ef67-117">String</span><span class="sxs-lookup"><span data-stu-id="2ef67-117">String</span></span>     |<span data-ttu-id="2ef67-118">Identificador de regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2ef67-118">Synchronization rule identifier.</span></span> <span data-ttu-id="2ef67-119">Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2ef67-119">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="2ef67-120">Os identificadores de regra suportados podem ser encontrados no modelo de sincronização retornado pela API.</span><span class="sxs-lookup"><span data-stu-id="2ef67-120">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="2ef67-121">los</span><span class="sxs-lookup"><span data-stu-id="2ef67-121">metadata</span></span>       |<span data-ttu-id="2ef67-122">coleção [stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2ef67-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="2ef67-123">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="2ef67-123">Additional extension properties.</span></span> <span data-ttu-id="2ef67-124">A menos que instruído explicitamente pela equipe de suporte, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="2ef67-124">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="2ef67-125">nome</span><span class="sxs-lookup"><span data-stu-id="2ef67-125">name</span></span>           |<span data-ttu-id="2ef67-126">String</span><span class="sxs-lookup"><span data-stu-id="2ef67-126">String</span></span>     |<span data-ttu-id="2ef67-127">Nome legível da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="2ef67-127">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="2ef67-128">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2ef67-128">Not nullable.</span></span>|
|<span data-ttu-id="2ef67-129">objectmappings</span><span class="sxs-lookup"><span data-stu-id="2ef67-129">objectMappings</span></span> |<span data-ttu-id="2ef67-130">coleção [Objectmapping](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="2ef67-130">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="2ef67-131">Conjunto de mapeamentos de objeto com suporte da regra.</span><span class="sxs-lookup"><span data-stu-id="2ef67-131">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="2ef67-132">Informa ao mecanismo de sincronização quais objetos devem ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="2ef67-132">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="2ef67-133">prioridade</span><span class="sxs-lookup"><span data-stu-id="2ef67-133">priority</span></span>       |<span data-ttu-id="2ef67-134">Inteiro</span><span class="sxs-lookup"><span data-stu-id="2ef67-134">Integer</span></span>    |<span data-ttu-id="2ef67-135">Prioridade relativa a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2ef67-135">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="2ef67-136">As regras com o número de prioridade mais baixa serão processadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="2ef67-136">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="2ef67-137">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="2ef67-137">sourceDirectoryName</span></span>       |<span data-ttu-id="2ef67-138">String</span><span class="sxs-lookup"><span data-stu-id="2ef67-138">String</span></span>    |<span data-ttu-id="2ef67-139">Nome do diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="2ef67-139">Name of the source directory.</span></span> <span data-ttu-id="2ef67-140">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2ef67-140">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="2ef67-141">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="2ef67-141">targetDirectoryName</span></span>       |<span data-ttu-id="2ef67-142">String</span><span class="sxs-lookup"><span data-stu-id="2ef67-142">String</span></span>    |<span data-ttu-id="2ef67-143">Nome do diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="2ef67-143">Name of the target directory.</span></span> <span data-ttu-id="2ef67-144">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2ef67-144">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ef67-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ef67-145">JSON representation</span></span>

<span data-ttu-id="2ef67-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ef67-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
