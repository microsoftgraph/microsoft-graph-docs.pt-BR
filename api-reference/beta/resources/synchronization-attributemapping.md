---
title: tipo de recurso de attributeMapping
description: Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641873"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="ab636-103">tipo de recurso de attributeMapping</span><span class="sxs-lookup"><span data-stu-id="ab636-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab636-104">Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="ab636-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="ab636-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab636-105">Properties</span></span>

| <span data-ttu-id="ab636-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab636-106">Property</span></span>                  | <span data-ttu-id="ab636-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab636-107">Type</span></span>                      | <span data-ttu-id="ab636-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab636-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="ab636-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="ab636-109">defaultValue</span></span>               | <span data-ttu-id="ab636-110">String</span><span class="sxs-lookup"><span data-stu-id="ab636-110">String</span></span>                    |<span data-ttu-id="ab636-111">Valor a ser usado caso a propriedade **source** foi avaliada como padrão `null`.</span><span class="sxs-lookup"><span data-stu-id="ab636-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="ab636-112">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ab636-112">Optional.</span></span>|
|<span data-ttu-id="ab636-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="ab636-113">exportMissingReferences</span></span>    |<span data-ttu-id="ab636-114">String</span><span class="sxs-lookup"><span data-stu-id="ab636-114">String</span></span>                     |<span data-ttu-id="ab636-115">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="ab636-115">For internal use only.</span></span>|
|<span data-ttu-id="ab636-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="ab636-116">flowBehavior</span></span>               |<span data-ttu-id="ab636-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="ab636-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="ab636-118">Define quando este atributo deve ser exportado para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="ab636-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="ab636-119">Os valores possíveis são: `FlowWhenChanged` e `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="ab636-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="ab636-120">O padrão é `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="ab636-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="ab636-121">flowType</span><span class="sxs-lookup"><span data-stu-id="ab636-121">flowType</span></span>                   |<span data-ttu-id="ab636-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="ab636-122">attributeFlowType</span></span>          |<span data-ttu-id="ab636-123">Define quando este atributo deve ser atualizado no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="ab636-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="ab636-124">Os valores possíveis são: `Always` (padrão), `ObjectAddOnly` (somente quando novo objeto é criado), `MultiValueAddOnly` (somente quando a alteração é adicionando novos valores para um atributo de valores múltiplos).</span><span class="sxs-lookup"><span data-stu-id="ab636-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="ab636-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="ab636-125">matchingPriority</span></span>           |<span data-ttu-id="ab636-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ab636-126">Int32</span></span>                      |<span data-ttu-id="ab636-127">Se for maior do que 0, esse atributo será usado para executar uma correspondência inicial dos objetos entre os diretórios de origem e destino.</span><span class="sxs-lookup"><span data-stu-id="ab636-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="ab636-128">O mecanismo de sincronização tentará localizar o objeto correspondente usando o atributo com menor valor de prioridade de correspondência pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="ab636-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="ab636-129">Se não encontrado, o atributo com a prioridade de correspondência próxima será usado e assim por diante um até correspondência for encontrada ou não mais atributos correspondentes são deixados.</span><span class="sxs-lookup"><span data-stu-id="ab636-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="ab636-130">Apenas os atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="ab636-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="ab636-131">source</span><span class="sxs-lookup"><span data-stu-id="ab636-131">source</span></span>                     |[<span data-ttu-id="ab636-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="ab636-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="ab636-133">Define como um valor deve ser extraída (ou transformados) do objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="ab636-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="ab636-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="ab636-134">targetAttributeName</span></span>        |<span data-ttu-id="ab636-135">String</span><span class="sxs-lookup"><span data-stu-id="ab636-135">String</span></span>                     |<span data-ttu-id="ab636-136">Nome do atributo no objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="ab636-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab636-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab636-137">JSON representation</span></span>

<span data-ttu-id="ab636-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab636-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
