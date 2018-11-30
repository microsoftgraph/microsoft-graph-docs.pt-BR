---
title: tipo de recurso de attributeMapping
description: Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.
ms.openlocfilehash: e4fd8ba0aece448f358d51373dfca0157759a23e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036510"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="3e566-103">tipo de recurso de attributeMapping</span><span class="sxs-lookup"><span data-stu-id="3e566-103">attributeMapping resource type</span></span>

> <span data-ttu-id="3e566-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e566-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e566-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e566-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e566-106">Define como os valores para o atributo de destino fornecido devem fluir durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="3e566-106">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="3e566-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e566-107">Properties</span></span>

| <span data-ttu-id="3e566-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e566-108">Property</span></span>                  | <span data-ttu-id="3e566-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e566-109">Type</span></span>                      | <span data-ttu-id="3e566-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e566-110">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="3e566-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="3e566-111">defaultValue</span></span>               | <span data-ttu-id="3e566-112">String</span><span class="sxs-lookup"><span data-stu-id="3e566-112">String</span></span>                    |<span data-ttu-id="3e566-113">Valor a ser usado caso a propriedade **source** foi avaliada como padrão `null`.</span><span class="sxs-lookup"><span data-stu-id="3e566-113">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="3e566-114">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3e566-114">Optional.</span></span>|
|<span data-ttu-id="3e566-115">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="3e566-115">exportMissingReferences</span></span>    |<span data-ttu-id="3e566-116">String</span><span class="sxs-lookup"><span data-stu-id="3e566-116">String</span></span>                     |<span data-ttu-id="3e566-117">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="3e566-117">For internal use only.</span></span>|
|<span data-ttu-id="3e566-118">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="3e566-118">flowBehavior</span></span>               |<span data-ttu-id="3e566-119">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="3e566-119">attributeFlowBehavior</span></span>      |<span data-ttu-id="3e566-120">Define quando este atributo deve ser exportado para o diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="3e566-120">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="3e566-121">Os valores possíveis são: `FlowWhenChanged` e `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="3e566-121">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="3e566-122">O padrão é `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="3e566-122">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="3e566-123">flowType</span><span class="sxs-lookup"><span data-stu-id="3e566-123">flowType</span></span>                   |<span data-ttu-id="3e566-124">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="3e566-124">attributeFlowType</span></span>          |<span data-ttu-id="3e566-125">Define quando este atributo deve ser atualizado no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="3e566-125">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="3e566-126">Os valores possíveis são: `Always` (padrão), `ObjectAddOnly` (somente quando novo objeto é criado), `MultiValueAddOnly` (somente quando a alteração é adicionando novos valores para um atributo de valores múltiplos).</span><span class="sxs-lookup"><span data-stu-id="3e566-126">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="3e566-127">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="3e566-127">matchingPriority</span></span>           |<span data-ttu-id="3e566-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3e566-128">Int32</span></span>                      |<span data-ttu-id="3e566-129">Se for maior do que 0, esse atributo será usado para executar uma correspondência inicial dos objetos entre os diretórios de origem e destino.</span><span class="sxs-lookup"><span data-stu-id="3e566-129">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="3e566-130">O mecanismo de sincronização tentará localizar o objeto correspondente usando o atributo com menor valor de prioridade de correspondência pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="3e566-130">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="3e566-131">Se não encontrado, o atributo com a prioridade de correspondência próxima será usado e assim por diante um até correspondência for encontrada ou não mais atributos correspondentes são deixados.</span><span class="sxs-lookup"><span data-stu-id="3e566-131">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="3e566-132">Apenas os atributos que devem ter valores exclusivos, como email, devem ser usados como atributos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="3e566-132">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="3e566-133">source</span><span class="sxs-lookup"><span data-stu-id="3e566-133">source</span></span>                     |[<span data-ttu-id="3e566-134">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="3e566-134">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="3e566-135">Define como um valor deve ser extraída (ou transformados) do objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="3e566-135">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="3e566-136">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="3e566-136">targetAttributeName</span></span>        |<span data-ttu-id="3e566-137">String</span><span class="sxs-lookup"><span data-stu-id="3e566-137">String</span></span>                     |<span data-ttu-id="3e566-138">Nome do atributo no objeto de destino.</span><span class="sxs-lookup"><span data-stu-id="3e566-138">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e566-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e566-139">JSON representation</span></span>

<span data-ttu-id="3e566-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e566-140">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->