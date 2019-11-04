---
title: tipo de recurso contentInfo
description: Representa o estado atual de algumas informações que serão rotuladas.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5191be0533810f0a9da3b0ea83f209d69cc67297
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938874"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="91107-103">tipo de recurso contentInfo</span><span class="sxs-lookup"><span data-stu-id="91107-103">contentInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91107-104">Representa o estado atual de algumas informações que serão rotuladas.</span><span class="sxs-lookup"><span data-stu-id="91107-104">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="91107-105">**contentInfo** é passado para as APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) para descrever a API o estado atual das informações.</span><span class="sxs-lookup"><span data-stu-id="91107-105">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="91107-106">Este detalhe de **contentInfo** orienta os resultados em quais metadados, a marcação de conteúdo e a proteção devem ser adicionados ou removidos quando o rótulo é aplicado, atualizado ou removido.</span><span class="sxs-lookup"><span data-stu-id="91107-106">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="91107-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91107-107">Properties</span></span>

| <span data-ttu-id="91107-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91107-108">Property</span></span>   | <span data-ttu-id="91107-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="91107-109">Type</span></span>                                       | <span data-ttu-id="91107-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="91107-110">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="91107-111">formato</span><span class="sxs-lookup"><span data-stu-id="91107-111">format</span></span>     | <span data-ttu-id="91107-112">String</span><span class="sxs-lookup"><span data-stu-id="91107-112">String</span></span>                                     | <span data-ttu-id="91107-113">Os valores possíveis são: `default` e `email`.</span><span class="sxs-lookup"><span data-stu-id="91107-113">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="91107-114">identificador</span><span class="sxs-lookup"><span data-stu-id="91107-114">identifier</span></span> | <span data-ttu-id="91107-115">String</span><span class="sxs-lookup"><span data-stu-id="91107-115">String</span></span>                                     | <span data-ttu-id="91107-116">Identificador usado para a análise de proteção de informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="91107-116">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="91107-117">los</span><span class="sxs-lookup"><span data-stu-id="91107-117">metadata</span></span>   | <span data-ttu-id="91107-118">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="91107-118">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="91107-119">Os metadados de proteção de informações existentes da Microsoft são passados como pares chave/valor, onde a chave é o MSIP_Label_GUID_PropName.</span><span class="sxs-lookup"><span data-stu-id="91107-119">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="91107-120">state</span><span class="sxs-lookup"><span data-stu-id="91107-120">state</span></span>      | <span data-ttu-id="91107-121">String</span><span class="sxs-lookup"><span data-stu-id="91107-121">String</span></span>                                     | <span data-ttu-id="91107-122">Os valores possíveis são: `rest`, `motion`, `use`.</span><span class="sxs-lookup"><span data-stu-id="91107-122">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="91107-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91107-123">JSON representation</span></span>

<span data-ttu-id="91107-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91107-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.contentInfo",
  "baseType": null
}-->

```json
{
  "format": "String",
  "identifier": "String",
  "metadata": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contentInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->