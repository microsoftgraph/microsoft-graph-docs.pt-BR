---
title: tipo de recurso synchronizationRule
description: Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos sincronizar e em que direção, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformada quando estiverem sincronizadas da origem para o diretório de destino.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 367c0f00fb4abe4a41785f3b73599c06a2b31d6f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007770"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="83821-103">tipo de recurso synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="83821-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83821-104">Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos sincronizar e em que direção, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformada quando estiverem sincronizadas da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="83821-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="83821-105">**Observação:** As regras de sincronização definem a sincronização em uma direção – do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="83821-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="83821-106">Os diretórios de origem e de destino são definidos como parte das propriedades da regra.</span><span class="sxs-lookup"><span data-stu-id="83821-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="83821-107">As regras de sincronização são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83821-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="83821-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83821-108">Properties</span></span>

| <span data-ttu-id="83821-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83821-109">Property</span></span>      | <span data-ttu-id="83821-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="83821-110">Type</span></span>      | <span data-ttu-id="83821-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83821-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="83821-112">edita</span><span class="sxs-lookup"><span data-stu-id="83821-112">editable</span></span>       |<span data-ttu-id="83821-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="83821-113">Boolean</span></span>    |<span data-ttu-id="83821-114">`true`se a regra de sincronização puder ser personalizada; `false` se essa regra é somente leitura e não deve ser alterada.</span><span class="sxs-lookup"><span data-stu-id="83821-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="83821-115">id</span><span class="sxs-lookup"><span data-stu-id="83821-115">id</span></span>             |<span data-ttu-id="83821-116">String</span><span class="sxs-lookup"><span data-stu-id="83821-116">String</span></span>     |<span data-ttu-id="83821-117">Identificador de regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="83821-117">Synchronization rule identifier.</span></span> <span data-ttu-id="83821-118">Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="83821-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="83821-119">Os identificadores de regra suportados podem ser encontrados no modelo de sincronização retornado pela API.</span><span class="sxs-lookup"><span data-stu-id="83821-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="83821-120">los</span><span class="sxs-lookup"><span data-stu-id="83821-120">metadata</span></span>       |<span data-ttu-id="83821-121">coleção [stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="83821-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="83821-122">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="83821-122">Additional extension properties.</span></span> <span data-ttu-id="83821-123">A menos que instruído explicitamente pela equipe de suporte, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="83821-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="83821-124">name</span><span class="sxs-lookup"><span data-stu-id="83821-124">name</span></span>           |<span data-ttu-id="83821-125">String</span><span class="sxs-lookup"><span data-stu-id="83821-125">String</span></span>     |<span data-ttu-id="83821-126">Nome legível da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="83821-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="83821-127">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="83821-127">Not nullable.</span></span>|
|<span data-ttu-id="83821-128">objectmappings</span><span class="sxs-lookup"><span data-stu-id="83821-128">objectMappings</span></span> |<span data-ttu-id="83821-129">[](synchronization-objectmapping.md) coleção objectmapping</span><span class="sxs-lookup"><span data-stu-id="83821-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="83821-130">Conjunto de mapeamentos de objeto com suporte da regra.</span><span class="sxs-lookup"><span data-stu-id="83821-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="83821-131">Informa ao mecanismo de sincronização quais objetos devem ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="83821-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="83821-132">prioridade</span><span class="sxs-lookup"><span data-stu-id="83821-132">priority</span></span>       |<span data-ttu-id="83821-133">Inteiro</span><span class="sxs-lookup"><span data-stu-id="83821-133">Integer</span></span>    |<span data-ttu-id="83821-134">Prioridade relativa a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83821-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="83821-135">As regras com o número de prioridade mais baixa serão processadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="83821-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="83821-136">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="83821-136">sourceDirectoryName</span></span>       |<span data-ttu-id="83821-137">String</span><span class="sxs-lookup"><span data-stu-id="83821-137">String</span></span>    |<span data-ttu-id="83821-138">Nome do diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="83821-138">Name of the source directory.</span></span> <span data-ttu-id="83821-139">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83821-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="83821-140">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="83821-140">targetDirectoryName</span></span>       |<span data-ttu-id="83821-141">String</span><span class="sxs-lookup"><span data-stu-id="83821-141">String</span></span>    |<span data-ttu-id="83821-142">Nome do diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="83821-142">Name of the target directory.</span></span> <span data-ttu-id="83821-143">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="83821-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83821-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83821-144">JSON representation</span></span>

<span data-ttu-id="83821-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83821-145">The following is a JSON representation of the resource.</span></span>

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
