---
title: tipo de recurso synchronizationRule
description: Define como a sincronização deve ser executada para o mecanismo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 86a5f39612b6fdbeb123a74372520115e0357fb0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023811"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="78d81-103">tipo de recurso synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="78d81-103">synchronizationRule resource type</span></span>

<span data-ttu-id="78d81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78d81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78d81-105">Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos sincronizar e em que direção, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos devem ser transformados quando forem sincronizados da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="78d81-105">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="78d81-106">**Observação:** As regras de sincronização definem a sincronização em uma direção – do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="78d81-106">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="78d81-107">Os diretórios de origem e de destino são definidos como parte das propriedades da regra.</span><span class="sxs-lookup"><span data-stu-id="78d81-107">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="78d81-108">As regras de sincronização são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="78d81-108">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="78d81-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78d81-109">Properties</span></span>

| <span data-ttu-id="78d81-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78d81-110">Property</span></span>      | <span data-ttu-id="78d81-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="78d81-111">Type</span></span>      | <span data-ttu-id="78d81-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="78d81-112">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="78d81-113">edita</span><span class="sxs-lookup"><span data-stu-id="78d81-113">editable</span></span>       |<span data-ttu-id="78d81-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="78d81-114">Boolean</span></span>    |<span data-ttu-id="78d81-115">`true` se a regra de sincronização puder ser personalizada; `false` se essa regra é somente leitura e não deve ser alterada.</span><span class="sxs-lookup"><span data-stu-id="78d81-115">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="78d81-116">id</span><span class="sxs-lookup"><span data-stu-id="78d81-116">id</span></span>             |<span data-ttu-id="78d81-117">String</span><span class="sxs-lookup"><span data-stu-id="78d81-117">String</span></span>     |<span data-ttu-id="78d81-118">Identificador de regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="78d81-118">Synchronization rule identifier.</span></span> <span data-ttu-id="78d81-119">Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="78d81-119">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="78d81-120">Os identificadores de regra suportados podem ser encontrados no modelo de sincronização retornado pela API.</span><span class="sxs-lookup"><span data-stu-id="78d81-120">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="78d81-121">los</span><span class="sxs-lookup"><span data-stu-id="78d81-121">metadata</span></span>       |<span data-ttu-id="78d81-122">coleção [stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="78d81-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="78d81-123">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="78d81-123">Additional extension properties.</span></span> <span data-ttu-id="78d81-124">A menos que instruído explicitamente pela equipe de suporte, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="78d81-124">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="78d81-125">nome</span><span class="sxs-lookup"><span data-stu-id="78d81-125">name</span></span>           |<span data-ttu-id="78d81-126">String</span><span class="sxs-lookup"><span data-stu-id="78d81-126">String</span></span>     |<span data-ttu-id="78d81-127">Nome legível da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="78d81-127">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="78d81-128">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="78d81-128">Not nullable.</span></span>|
|<span data-ttu-id="78d81-129">objectmappings</span><span class="sxs-lookup"><span data-stu-id="78d81-129">objectMappings</span></span> |<span data-ttu-id="78d81-130">coleção [Objectmapping](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="78d81-130">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="78d81-131">Conjunto de mapeamentos de objeto com suporte da regra.</span><span class="sxs-lookup"><span data-stu-id="78d81-131">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="78d81-132">Informa ao mecanismo de sincronização quais objetos devem ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="78d81-132">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="78d81-133">prioridade</span><span class="sxs-lookup"><span data-stu-id="78d81-133">priority</span></span>       |<span data-ttu-id="78d81-134">Inteiro</span><span class="sxs-lookup"><span data-stu-id="78d81-134">Integer</span></span>    |<span data-ttu-id="78d81-135">Prioridade relativa a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="78d81-135">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="78d81-136">As regras com o número de prioridade mais baixa serão processadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="78d81-136">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="78d81-137">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="78d81-137">sourceDirectoryName</span></span>       |<span data-ttu-id="78d81-138">String</span><span class="sxs-lookup"><span data-stu-id="78d81-138">String</span></span>    |<span data-ttu-id="78d81-139">Nome do diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="78d81-139">Name of the source directory.</span></span> <span data-ttu-id="78d81-140">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="78d81-140">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="78d81-141">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="78d81-141">targetDirectoryName</span></span>       |<span data-ttu-id="78d81-142">String</span><span class="sxs-lookup"><span data-stu-id="78d81-142">String</span></span>    |<span data-ttu-id="78d81-143">Nome do diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="78d81-143">Name of the target directory.</span></span> <span data-ttu-id="78d81-144">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="78d81-144">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78d81-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78d81-145">JSON representation</span></span>

<span data-ttu-id="78d81-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78d81-146">The following is a JSON representation of the resource.</span></span>

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


