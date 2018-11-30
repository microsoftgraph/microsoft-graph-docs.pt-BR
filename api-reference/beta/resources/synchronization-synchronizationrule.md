---
title: tipo de recurso de synchronizationRule
description: Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos para sincronizar e na direção, como objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformados quando elas estiver sincronizadas da origem para o diretório de destino.
ms.openlocfilehash: c860228637a6cc3ad9137851408379bd7f779c75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035076"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="1ef18-103">tipo de recurso de synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="1ef18-103">synchronizationRule resource type</span></span>

> <span data-ttu-id="1ef18-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1ef18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ef18-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1ef18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ef18-106">Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos para sincronizar e na direção, como objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformados quando elas estiver sincronizadas da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="1ef18-106">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="1ef18-107">**Observação:** Regras de sincronização definem sincronização em uma direção - do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="1ef18-107">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="1ef18-108">Os diretórios de origem e destino são definidos como parte das propriedades de regra.</span><span class="sxs-lookup"><span data-stu-id="1ef18-108">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="1ef18-109">Regras de sincronização são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1ef18-109">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1ef18-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ef18-110">Properties</span></span>

| <span data-ttu-id="1ef18-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ef18-111">Property</span></span>      | <span data-ttu-id="1ef18-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ef18-112">Type</span></span>      | <span data-ttu-id="1ef18-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ef18-113">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="1ef18-114">editável</span><span class="sxs-lookup"><span data-stu-id="1ef18-114">editable</span></span>       |<span data-ttu-id="1ef18-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ef18-115">Boolean</span></span>    |<span data-ttu-id="1ef18-116">`true`Se a regra de sincronização pode ser personalizada; `false` se esta regra é somente leitura e não deve ser alterada.</span><span class="sxs-lookup"><span data-stu-id="1ef18-116">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="1ef18-117">id</span><span class="sxs-lookup"><span data-stu-id="1ef18-117">id</span></span>             |<span data-ttu-id="1ef18-118">String</span><span class="sxs-lookup"><span data-stu-id="1ef18-118">String</span></span>     |<span data-ttu-id="1ef18-119">Identificador da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1ef18-119">Synchronization rule identifier.</span></span> <span data-ttu-id="1ef18-120">Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1ef18-120">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="1ef18-121">Suporte para a regra identificadores podem ser encontrados no modelo de sincronização retornado pela API.</span><span class="sxs-lookup"><span data-stu-id="1ef18-121">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="1ef18-122">metadados</span><span class="sxs-lookup"><span data-stu-id="1ef18-122">metadata</span></span>       |<span data-ttu-id="1ef18-123">coleção [stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1ef18-123">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="1ef18-124">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="1ef18-124">Additional extension properties.</span></span> <span data-ttu-id="1ef18-125">A menos que seja instruído explicitamente pela equipe de suporte, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="1ef18-125">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="1ef18-126">name</span><span class="sxs-lookup"><span data-stu-id="1ef18-126">name</span></span>           |<span data-ttu-id="1ef18-127">String</span><span class="sxs-lookup"><span data-stu-id="1ef18-127">String</span></span>     |<span data-ttu-id="1ef18-128">Legíveis nome da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1ef18-128">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="1ef18-129">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="1ef18-129">Not nullable.</span></span>|
|<span data-ttu-id="1ef18-130">objectMappings</span><span class="sxs-lookup"><span data-stu-id="1ef18-130">objectMappings</span></span> |<span data-ttu-id="1ef18-131">coleção [objectMapping](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="1ef18-131">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="1ef18-132">Conjunto de mapeamentos de objeto suportado pela regra.</span><span class="sxs-lookup"><span data-stu-id="1ef18-132">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="1ef18-133">Instrui o mecanismo de sincronização quais objetos devem ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="1ef18-133">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="1ef18-134">prioridade</span><span class="sxs-lookup"><span data-stu-id="1ef18-134">priority</span></span>       |<span data-ttu-id="1ef18-135">Inteiro</span><span class="sxs-lookup"><span data-stu-id="1ef18-135">Integer</span></span>    |<span data-ttu-id="1ef18-136">Prioridade em relação a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1ef18-136">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="1ef18-137">As regras com o número de prioridade mais baixa serão processadas pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="1ef18-137">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="1ef18-138">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="1ef18-138">sourceDirectoryName</span></span>       |<span data-ttu-id="1ef18-139">String</span><span class="sxs-lookup"><span data-stu-id="1ef18-139">String</span></span>    |<span data-ttu-id="1ef18-140">Nome do diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="1ef18-140">Name of the source directory.</span></span> <span data-ttu-id="1ef18-141">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1ef18-141">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="1ef18-142">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="1ef18-142">targetDirectoryName</span></span>       |<span data-ttu-id="1ef18-143">String</span><span class="sxs-lookup"><span data-stu-id="1ef18-143">String</span></span>    |<span data-ttu-id="1ef18-144">Nome do diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="1ef18-144">Name of the target directory.</span></span> <span data-ttu-id="1ef18-145">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1ef18-145">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ef18-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ef18-146">JSON representation</span></span>

<span data-ttu-id="1ef18-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ef18-147">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->