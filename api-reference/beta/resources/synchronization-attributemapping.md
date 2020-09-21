---
title: tipo de recurso attributeMapping
description: Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7573773737f4ff4380a446cf62107e8ac26642ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078077"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="076a5-103">tipo de recurso attributeMapping</span><span class="sxs-lookup"><span data-stu-id="076a5-103">attributeMapping resource type</span></span>

<span data-ttu-id="076a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="076a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="076a5-105">Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="076a5-105">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="076a5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="076a5-106">Properties</span></span>

| <span data-ttu-id="076a5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="076a5-107">Property</span></span>                  | <span data-ttu-id="076a5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="076a5-108">Type</span></span>                      | <span data-ttu-id="076a5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="076a5-109">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="076a5-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="076a5-110">defaultValue</span></span>               | <span data-ttu-id="076a5-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="076a5-111">String</span></span>                    |<span data-ttu-id="076a5-112">Valor padrão a ser usado no caso de a propriedade **Source** ter sido avaliada `null` .</span><span class="sxs-lookup"><span data-stu-id="076a5-112">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="076a5-113">Opcional.</span><span class="sxs-lookup"><span data-stu-id="076a5-113">Optional.</span></span>|
|<span data-ttu-id="076a5-114">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="076a5-114">exportMissingReferences</span></span>    |<span data-ttu-id="076a5-115">String</span><span class="sxs-lookup"><span data-stu-id="076a5-115">String</span></span>                     |<span data-ttu-id="076a5-116">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="076a5-116">For internal use only.</span></span>|
|<span data-ttu-id="076a5-117">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="076a5-117">flowBehavior</span></span>               |<span data-ttu-id="076a5-118">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="076a5-118">attributeFlowBehavior</span></span>      |<span data-ttu-id="076a5-119">Define quando esse atributo deve ser exportado para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="076a5-119">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="076a5-120">Os valores possíveis são: `FlowWhenChanged` e `FlowAlways` .</span><span class="sxs-lookup"><span data-stu-id="076a5-120">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="076a5-121">O padrão é `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="076a5-121">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="076a5-122">flowtype</span><span class="sxs-lookup"><span data-stu-id="076a5-122">flowType</span></span>                   |<span data-ttu-id="076a5-123">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="076a5-123">attributeFlowType</span></span>          |<span data-ttu-id="076a5-124">Define quando esse atributo deve ser atualizado no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="076a5-124">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="076a5-125">Os valores possíveis são: `Always` (padrão), `ObjectAddOnly` (somente quando novo objeto é criado), `MultiValueAddOnly` (somente quando a alteração está adicionando novos valores a um atributo com valores múltiplos).</span><span class="sxs-lookup"><span data-stu-id="076a5-125">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="076a5-126">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="076a5-126">matchingPriority</span></span>           |<span data-ttu-id="076a5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="076a5-127">Int32</span></span>                      |<span data-ttu-id="076a5-128">Se for maior que 0, este atributo será usado para executar uma correspondência inicial dos objetos entre os diretórios de origem e de destino.</span><span class="sxs-lookup"><span data-stu-id="076a5-128">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="076a5-129">O mecanismo de sincronização tentará localizar o objeto correspondente usando o atributo com o menor valor de prioridade correspondente primeiro.</span><span class="sxs-lookup"><span data-stu-id="076a5-129">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="076a5-130">Se não for encontrado, será usado o atributo com a próxima prioridade correspondente e, assim, em um até que a correspondência seja encontrada ou nenhum outro atributo de correspondência seja deixado.</span><span class="sxs-lookup"><span data-stu-id="076a5-130">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="076a5-131">Somente atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="076a5-131">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="076a5-132">source</span><span class="sxs-lookup"><span data-stu-id="076a5-132">source</span></span>                     |[<span data-ttu-id="076a5-133">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="076a5-133">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="076a5-134">Define como um valor deve ser extraído (ou transformado) a partir do objeto Source.</span><span class="sxs-lookup"><span data-stu-id="076a5-134">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="076a5-135">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="076a5-135">targetAttributeName</span></span>        |<span data-ttu-id="076a5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="076a5-136">String</span></span>                     |<span data-ttu-id="076a5-137">Nome do atributo no objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="076a5-137">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="076a5-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="076a5-138">JSON representation</span></span>

<span data-ttu-id="076a5-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="076a5-139">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


