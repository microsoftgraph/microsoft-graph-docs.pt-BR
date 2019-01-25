---
title: tipo de recurso de synchronizationRule
description: Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos para sincronizar e na direção, como objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformados quando elas estiver sincronizadas da origem para o diretório de destino.
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517922"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="fe1f8-103">tipo de recurso de synchronizationRule</span><span class="sxs-lookup"><span data-stu-id="fe1f8-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe1f8-104">Define como a sincronização deve ser executada para o mecanismo de sincronização, incluindo quais objetos para sincronizar e na direção, como objetos do diretório de origem devem ser correspondidos com objetos no diretório de destino e como os atributos deve ser transformados quando elas estiver sincronizadas da origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="fe1f8-105">**Observação:** Regras de sincronização definem sincronização em uma direção - do diretório de origem para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="fe1f8-106">Os diretórios de origem e destino são definidos como parte das propriedades de regra.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="fe1f8-107">Regras de sincronização são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fe1f8-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fe1f8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe1f8-108">Properties</span></span>

| <span data-ttu-id="fe1f8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe1f8-109">Property</span></span>      | <span data-ttu-id="fe1f8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe1f8-110">Type</span></span>      | <span data-ttu-id="fe1f8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe1f8-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="fe1f8-112">Editable</span><span class="sxs-lookup"><span data-stu-id="fe1f8-112">editable</span></span>       |<span data-ttu-id="fe1f8-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="fe1f8-113">Boolean</span></span>    |<span data-ttu-id="fe1f8-114">`true`Se a regra de sincronização pode ser personalizada; `false` se esta regra é somente leitura e não deve ser alterada.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="fe1f8-115">id</span><span class="sxs-lookup"><span data-stu-id="fe1f8-115">id</span></span>             |<span data-ttu-id="fe1f8-116">String</span><span class="sxs-lookup"><span data-stu-id="fe1f8-116">String</span></span>     |<span data-ttu-id="fe1f8-117">Identificador da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-117">Synchronization rule identifier.</span></span> <span data-ttu-id="fe1f8-118">Deve ser um dos identificadores reconhecidos pelo mecanismo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="fe1f8-119">Suporte para a regra identificadores podem ser encontrados no modelo de sincronização retornado pela API.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="fe1f8-120">Metadata</span><span class="sxs-lookup"><span data-stu-id="fe1f8-120">metadata</span></span>       |<span data-ttu-id="fe1f8-121">coleção [stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fe1f8-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="fe1f8-122">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-122">Additional extension properties.</span></span> <span data-ttu-id="fe1f8-123">A menos que seja instruído explicitamente pela equipe de suporte, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="fe1f8-124">name</span><span class="sxs-lookup"><span data-stu-id="fe1f8-124">name</span></span>           |<span data-ttu-id="fe1f8-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe1f8-125">String</span></span>     |<span data-ttu-id="fe1f8-126">Legíveis nome da regra de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="fe1f8-127">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-127">Not nullable.</span></span>|
|<span data-ttu-id="fe1f8-128">objectMappings</span><span class="sxs-lookup"><span data-stu-id="fe1f8-128">objectMappings</span></span> |<span data-ttu-id="fe1f8-129">coleção [objectMapping](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="fe1f8-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="fe1f8-130">Conjunto de mapeamentos de objeto suportado pela regra.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="fe1f8-131">Instrui o mecanismo de sincronização quais objetos devem ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="fe1f8-132">prioridade</span><span class="sxs-lookup"><span data-stu-id="fe1f8-132">priority</span></span>       |<span data-ttu-id="fe1f8-133">Inteiro</span><span class="sxs-lookup"><span data-stu-id="fe1f8-133">Integer</span></span>    |<span data-ttu-id="fe1f8-134">Prioridade em relação a outras regras no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fe1f8-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="fe1f8-135">As regras com o número de prioridade mais baixa serão processadas pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="fe1f8-136">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="fe1f8-136">sourceDirectoryName</span></span>       |<span data-ttu-id="fe1f8-137">String</span><span class="sxs-lookup"><span data-stu-id="fe1f8-137">String</span></span>    |<span data-ttu-id="fe1f8-138">Nome do diretório de origem.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-138">Name of the source directory.</span></span> <span data-ttu-id="fe1f8-139">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fe1f8-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="fe1f8-140">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="fe1f8-140">targetDirectoryName</span></span>       |<span data-ttu-id="fe1f8-141">String</span><span class="sxs-lookup"><span data-stu-id="fe1f8-141">String</span></span>    |<span data-ttu-id="fe1f8-142">Nome do diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-142">Name of the target directory.</span></span> <span data-ttu-id="fe1f8-143">Deve corresponder a uma das definições de diretório no [synchronizationSchema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fe1f8-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe1f8-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe1f8-144">JSON representation</span></span>

<span data-ttu-id="fe1f8-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe1f8-145">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationrule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
