---
title: Tipo de recurso attributeMapping
description: Define como os valores para o atributo de destino determinado devem fluir durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b5f120075b082e50a0f94f05907b413a4c4c4ec6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128747"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="eb269-103">Tipo de recurso attributeMapping</span><span class="sxs-lookup"><span data-stu-id="eb269-103">attributeMapping resource type</span></span>

<span data-ttu-id="eb269-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb269-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb269-105">Define como os valores para o atributo de destino determinado devem fluir durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="eb269-105">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="eb269-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb269-106">Properties</span></span>

| <span data-ttu-id="eb269-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb269-107">Property</span></span>                  | <span data-ttu-id="eb269-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb269-108">Type</span></span>                      | <span data-ttu-id="eb269-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb269-109">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="eb269-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="eb269-110">defaultValue</span></span>               | <span data-ttu-id="eb269-111">String</span><span class="sxs-lookup"><span data-stu-id="eb269-111">String</span></span>                    |<span data-ttu-id="eb269-112">Valor padrão a ser usado no caso de a **propriedade de origem** ter sido avaliada como `null` .</span><span class="sxs-lookup"><span data-stu-id="eb269-112">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="eb269-113">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb269-113">Optional.</span></span>|
|<span data-ttu-id="eb269-114">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="eb269-114">exportMissingReferences</span></span>    |<span data-ttu-id="eb269-115">String</span><span class="sxs-lookup"><span data-stu-id="eb269-115">String</span></span>                     |<span data-ttu-id="eb269-116">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="eb269-116">For internal use only.</span></span>|
|<span data-ttu-id="eb269-117">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="eb269-117">flowBehavior</span></span>               |<span data-ttu-id="eb269-118">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="eb269-118">attributeFlowBehavior</span></span>      |<span data-ttu-id="eb269-119">Define quando esse atributo deve ser exportado para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="eb269-119">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="eb269-120">Os valores possíveis são: `FlowWhenChanged` e `FlowAlways` .</span><span class="sxs-lookup"><span data-stu-id="eb269-120">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="eb269-121">O padrão é `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="eb269-121">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="eb269-122">flowType</span><span class="sxs-lookup"><span data-stu-id="eb269-122">flowType</span></span>                   |<span data-ttu-id="eb269-123">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="eb269-123">attributeFlowType</span></span>          |<span data-ttu-id="eb269-124">Define quando esse atributo deve ser atualizado no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="eb269-124">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="eb269-125">Os valores possíveis são: (padrão), (somente quando um novo objeto é criado) (somente quando a alteração está adicionando novos valores a um atributo `Always` `ObjectAddOnly` de vários `MultiValueAddOnly` valores).</span><span class="sxs-lookup"><span data-stu-id="eb269-125">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="eb269-126">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="eb269-126">matchingPriority</span></span>           |<span data-ttu-id="eb269-127">Int32</span><span class="sxs-lookup"><span data-stu-id="eb269-127">Int32</span></span>                      |<span data-ttu-id="eb269-128">Se for maior que 0, esse atributo será usado para executar uma combinação inicial dos objetos entre diretórios de origem e de destino.</span><span class="sxs-lookup"><span data-stu-id="eb269-128">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="eb269-129">O mecanismo de sincronização tentará encontrar o objeto correspondente usando primeiro o atributo com o menor valor de prioridade correspondente.</span><span class="sxs-lookup"><span data-stu-id="eb269-129">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="eb269-130">Se não for encontrado, o atributo com a próxima prioridade correspondente será usado e assim por diante até que uma correspondência seja encontrada ou mais atributos correspondentes sejam deixados.</span><span class="sxs-lookup"><span data-stu-id="eb269-130">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="eb269-131">Somente atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="eb269-131">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="eb269-132">source</span><span class="sxs-lookup"><span data-stu-id="eb269-132">source</span></span>                     |[<span data-ttu-id="eb269-133">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="eb269-133">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="eb269-134">Define como um valor deve ser extraído (ou transformado) do objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="eb269-134">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="eb269-135">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="eb269-135">targetAttributeName</span></span>        |<span data-ttu-id="eb269-136">String</span><span class="sxs-lookup"><span data-stu-id="eb269-136">String</span></span>                     |<span data-ttu-id="eb269-137">Nome do atributo no objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="eb269-137">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eb269-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb269-138">JSON representation</span></span>

<span data-ttu-id="eb269-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb269-139">The following is a JSON representation of the resource.</span></span>

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


