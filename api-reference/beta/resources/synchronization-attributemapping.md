---
title: tipo de recurso de attributeMapping
description: Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: 9f33aa9a784ba3e40fd8d38650737a9064a0831c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573659"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="a96cb-103">tipo de recurso de attributeMapping</span><span class="sxs-lookup"><span data-stu-id="a96cb-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a96cb-104">Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="a96cb-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="a96cb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a96cb-105">Properties</span></span>

| <span data-ttu-id="a96cb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a96cb-106">Property</span></span>                  | <span data-ttu-id="a96cb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a96cb-107">Type</span></span>                      | <span data-ttu-id="a96cb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a96cb-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="a96cb-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="a96cb-109">defaultValue</span></span>               | <span data-ttu-id="a96cb-110">String</span><span class="sxs-lookup"><span data-stu-id="a96cb-110">String</span></span>                    |<span data-ttu-id="a96cb-111">Valor a ser usado caso a propriedade **source** foi avaliada como padrão `null`.</span><span class="sxs-lookup"><span data-stu-id="a96cb-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="a96cb-112">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a96cb-112">Optional.</span></span>|
|<span data-ttu-id="a96cb-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="a96cb-113">exportMissingReferences</span></span>    |<span data-ttu-id="a96cb-114">String</span><span class="sxs-lookup"><span data-stu-id="a96cb-114">String</span></span>                     |<span data-ttu-id="a96cb-115">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="a96cb-115">For internal use only.</span></span>|
|<span data-ttu-id="a96cb-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="a96cb-116">flowBehavior</span></span>               | <span data-ttu-id="a96cb-117">cadeia de caracteres de enum</span><span class="sxs-lookup"><span data-stu-id="a96cb-117">enum-string</span></span>      |<span data-ttu-id="a96cb-118">Define quando este atributo deve ser exportado para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="a96cb-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="a96cb-119">Os valores possíveis são: `FlowWhenChanged` e `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="a96cb-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="a96cb-120">O padrão é `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="a96cb-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="a96cb-121">flowType</span><span class="sxs-lookup"><span data-stu-id="a96cb-121">flowType</span></span>                   | <span data-ttu-id="a96cb-122">cadeia de caracteres de ennum</span><span class="sxs-lookup"><span data-stu-id="a96cb-122">ennum-string</span></span>          |<span data-ttu-id="a96cb-123">Define quando este atributo deve ser atualizado no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="a96cb-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="a96cb-124">Os valores possíveis são: `Always` (padrão), `ObjectAddOnly` (somente quando novo objeto é criado), `MultiValueAddOnly` (somente quando a alteração é adicionando novos valores para um atributo de valores múltiplos).</span><span class="sxs-lookup"><span data-stu-id="a96cb-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="a96cb-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="a96cb-125">matchingPriority</span></span>           |<span data-ttu-id="a96cb-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a96cb-126">Int32</span></span>                      |<span data-ttu-id="a96cb-127">Se for maior do que 0, esse atributo será usado para executar uma correspondência inicial dos objetos entre os diretórios de origem e destino.</span><span class="sxs-lookup"><span data-stu-id="a96cb-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="a96cb-128">O mecanismo de sincronização tentará localizar o objeto correspondente usando o atributo com menor valor de prioridade de correspondência pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="a96cb-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="a96cb-129">Se não encontrado, o atributo com a prioridade de correspondência próxima será usado e assim por diante um até correspondência for encontrada ou não mais atributos correspondentes são deixados.</span><span class="sxs-lookup"><span data-stu-id="a96cb-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="a96cb-130">Apenas os atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="a96cb-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="a96cb-131">source</span><span class="sxs-lookup"><span data-stu-id="a96cb-131">source</span></span>                     |[<span data-ttu-id="a96cb-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="a96cb-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="a96cb-133">Define como um valor deve ser extraída (ou transformados) do objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="a96cb-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="a96cb-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="a96cb-134">targetAttributeName</span></span>        |<span data-ttu-id="a96cb-135">String</span><span class="sxs-lookup"><span data-stu-id="a96cb-135">String</span></span>                     |<span data-ttu-id="a96cb-136">Nome do atributo no objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="a96cb-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a96cb-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a96cb-137">JSON representation</span></span>

<span data-ttu-id="a96cb-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a96cb-138">The following is a JSON representation of the resource.</span></span>

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
  "flowBehavior": "FlowWhenChanged | FlowAlways",
  "flowType": "Always |  ObjectAddOnly | MultiValueAddOnly ",
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
