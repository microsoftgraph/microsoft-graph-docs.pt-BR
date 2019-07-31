---
title: tipo de recurso attributeMapping
description: Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 09ed298022e687354f7fa9905ee25f5c38f2fdfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964817"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="02ea9-103">tipo de recurso attributeMapping</span><span class="sxs-lookup"><span data-stu-id="02ea9-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02ea9-104">Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="02ea9-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="02ea9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02ea9-105">Properties</span></span>

| <span data-ttu-id="02ea9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02ea9-106">Property</span></span>                  | <span data-ttu-id="02ea9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="02ea9-107">Type</span></span>                      | <span data-ttu-id="02ea9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="02ea9-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="02ea9-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="02ea9-109">defaultValue</span></span>               | <span data-ttu-id="02ea9-110">String</span><span class="sxs-lookup"><span data-stu-id="02ea9-110">String</span></span>                    |<span data-ttu-id="02ea9-111">Valor padrão a ser usado no caso de a propriedade **Source** ter sido `null`avaliada.</span><span class="sxs-lookup"><span data-stu-id="02ea9-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="02ea9-112">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02ea9-112">Optional.</span></span>|
|<span data-ttu-id="02ea9-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="02ea9-113">exportMissingReferences</span></span>    |<span data-ttu-id="02ea9-114">String</span><span class="sxs-lookup"><span data-stu-id="02ea9-114">String</span></span>                     |<span data-ttu-id="02ea9-115">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="02ea9-115">For internal use only.</span></span>|
|<span data-ttu-id="02ea9-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="02ea9-116">flowBehavior</span></span>               |<span data-ttu-id="02ea9-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="02ea9-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="02ea9-118">Define quando esse atributo deve ser exportado para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="02ea9-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="02ea9-119">Os valores possíveis são `FlowWhenChanged` : `FlowAlways`e.</span><span class="sxs-lookup"><span data-stu-id="02ea9-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="02ea9-120">O padrão é `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="02ea9-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="02ea9-121">flowtype</span><span class="sxs-lookup"><span data-stu-id="02ea9-121">flowType</span></span>                   |<span data-ttu-id="02ea9-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="02ea9-122">attributeFlowType</span></span>          |<span data-ttu-id="02ea9-123">Define quando esse atributo deve ser atualizado no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="02ea9-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="02ea9-124">Os valores possíveis são `Always` : (padrão) `ObjectAddOnly` , (somente quando novo objeto é criado) `MultiValueAddOnly` , (somente quando a alteração está adicionando novos valores a um atributo com valores múltiplos).</span><span class="sxs-lookup"><span data-stu-id="02ea9-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="02ea9-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="02ea9-125">matchingPriority</span></span>           |<span data-ttu-id="02ea9-126">Int32</span><span class="sxs-lookup"><span data-stu-id="02ea9-126">Int32</span></span>                      |<span data-ttu-id="02ea9-127">Se for maior que 0, este atributo será usado para executar uma correspondência inicial dos objetos entre os diretórios de origem e de destino.</span><span class="sxs-lookup"><span data-stu-id="02ea9-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="02ea9-128">O mecanismo de sincronização tentará localizar o objeto correspondente usando o atributo com o menor valor de prioridade correspondente primeiro.</span><span class="sxs-lookup"><span data-stu-id="02ea9-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="02ea9-129">Se não for encontrado, será usado o atributo com a próxima prioridade correspondente e, assim, em um até que a correspondência seja encontrada ou nenhum outro atributo de correspondência seja deixado.</span><span class="sxs-lookup"><span data-stu-id="02ea9-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="02ea9-130">Somente atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="02ea9-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="02ea9-131">source</span><span class="sxs-lookup"><span data-stu-id="02ea9-131">source</span></span>                     |[<span data-ttu-id="02ea9-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="02ea9-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="02ea9-133">Define como um valor deve ser extraído (ou transformado) a partir do objeto Source.</span><span class="sxs-lookup"><span data-stu-id="02ea9-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="02ea9-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="02ea9-134">targetAttributeName</span></span>        |<span data-ttu-id="02ea9-135">String</span><span class="sxs-lookup"><span data-stu-id="02ea9-135">String</span></span>                     |<span data-ttu-id="02ea9-136">Nome do atributo no objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="02ea9-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02ea9-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02ea9-137">JSON representation</span></span>

<span data-ttu-id="02ea9-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02ea9-138">The following is a JSON representation of the resource.</span></span>

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
