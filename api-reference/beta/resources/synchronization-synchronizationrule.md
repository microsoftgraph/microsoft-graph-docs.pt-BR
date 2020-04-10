---
title: tipo de recurso synchronizationRule
description: Define como a sincronização deve ser executada para o mecanismo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0698afb7e3584aa1d4cd6697504138f6262e5141
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217364"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="8703c-103">tipo de recurso synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="8703c-103">synchronizationRule resource type</span></span>

<span data-ttu-id="8703c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8703c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8703c-105">Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos sincronizar e em que direção, como os objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos devem ser transformados quando forem sincronizados da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="8703c-105">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="8703c-106">**Observação:** As regras de sincronização definem a sincronização em uma direção – do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="8703c-106">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="8703c-107">Os diretórios de origem e de destino são definidos como parte das propriedades da regra.</span><span class="sxs-lookup"><span data-stu-id="8703c-107">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="8703c-108">As regras de sincronização são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8703c-108">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8703c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8703c-109">Properties</span></span>

| <span data-ttu-id="8703c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8703c-110">Property</span></span>      | <span data-ttu-id="8703c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8703c-111">Type</span></span>      | <span data-ttu-id="8703c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8703c-112">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="8703c-113">edita</span><span class="sxs-lookup"><span data-stu-id="8703c-113">editable</span></span>       |<span data-ttu-id="8703c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8703c-114">Boolean</span></span>    |<span data-ttu-id="8703c-115">`true`se a regra de sincronização puder ser personalizada; `false` se essa regra é somente leitura e não deve ser alterada.</span><span class="sxs-lookup"><span data-stu-id="8703c-115">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="8703c-116">id</span><span class="sxs-lookup"><span data-stu-id="8703c-116">id</span></span>             |<span data-ttu-id="8703c-117">String</span><span class="sxs-lookup"><span data-stu-id="8703c-117">String</span></span>     |<span data-ttu-id="8703c-118">Identificador de regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8703c-118">Synchronization rule identifier.</span></span> <span data-ttu-id="8703c-119">Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8703c-119">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="8703c-120">Os identificadores de regra suportados podem ser encontrados no modelo de sincronização retornado pela API.</span><span class="sxs-lookup"><span data-stu-id="8703c-120">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="8703c-121">los</span><span class="sxs-lookup"><span data-stu-id="8703c-121">metadata</span></span>       |<span data-ttu-id="8703c-122">coleção [stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8703c-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="8703c-123">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="8703c-123">Additional extension properties.</span></span> <span data-ttu-id="8703c-124">A menos que instruído explicitamente pela equipe de suporte, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="8703c-124">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="8703c-125">nome</span><span class="sxs-lookup"><span data-stu-id="8703c-125">name</span></span>           |<span data-ttu-id="8703c-126">String</span><span class="sxs-lookup"><span data-stu-id="8703c-126">String</span></span>     |<span data-ttu-id="8703c-127">Nome legível da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8703c-127">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="8703c-128">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="8703c-128">Not nullable.</span></span>|
|<span data-ttu-id="8703c-129">objectmappings</span><span class="sxs-lookup"><span data-stu-id="8703c-129">objectMappings</span></span> |<span data-ttu-id="8703c-130">coleção [Objectmapping](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="8703c-130">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="8703c-131">Conjunto de mapeamentos de objeto com suporte da regra.</span><span class="sxs-lookup"><span data-stu-id="8703c-131">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="8703c-132">Informa ao mecanismo de sincronização quais objetos devem ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="8703c-132">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="8703c-133">prioridade</span><span class="sxs-lookup"><span data-stu-id="8703c-133">priority</span></span>       |<span data-ttu-id="8703c-134">Inteiro</span><span class="sxs-lookup"><span data-stu-id="8703c-134">Integer</span></span>    |<span data-ttu-id="8703c-135">Prioridade relativa a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8703c-135">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="8703c-136">As regras com o número de prioridade mais baixa serão processadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="8703c-136">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="8703c-137">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="8703c-137">sourceDirectoryName</span></span>       |<span data-ttu-id="8703c-138">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8703c-138">String</span></span>    |<span data-ttu-id="8703c-139">Nome do diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="8703c-139">Name of the source directory.</span></span> <span data-ttu-id="8703c-140">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8703c-140">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="8703c-141">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="8703c-141">targetDirectoryName</span></span>       |<span data-ttu-id="8703c-142">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8703c-142">String</span></span>    |<span data-ttu-id="8703c-143">Nome do diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="8703c-143">Name of the target directory.</span></span> <span data-ttu-id="8703c-144">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8703c-144">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8703c-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8703c-145">JSON representation</span></span>

<span data-ttu-id="8703c-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8703c-146">The following is a JSON representation of the resource.</span></span>

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
