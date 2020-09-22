---
title: tipo de recurso contentInfo
description: Representa o estado atual de algumas informações que serão rotuladas.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d7e0c159d46cb680329efc6a93896ca3df7270f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998904"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="238a3-103">tipo de recurso contentInfo</span><span class="sxs-lookup"><span data-stu-id="238a3-103">contentInfo resource type</span></span>

<span data-ttu-id="238a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="238a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="238a3-105">Representa o estado atual de algumas informações que serão rotuladas.</span><span class="sxs-lookup"><span data-stu-id="238a3-105">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="238a3-106">**contentInfo** é passado para as APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) para descrever a API o estado atual das informações.</span><span class="sxs-lookup"><span data-stu-id="238a3-106">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="238a3-107">Este detalhe de **contentInfo** orienta os resultados em quais metadados, a marcação de conteúdo e a proteção devem ser adicionados ou removidos quando o rótulo é aplicado, atualizado ou removido.</span><span class="sxs-lookup"><span data-stu-id="238a3-107">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="238a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="238a3-108">Properties</span></span>

| <span data-ttu-id="238a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="238a3-109">Property</span></span>   | <span data-ttu-id="238a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="238a3-110">Type</span></span>                                       | <span data-ttu-id="238a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="238a3-111">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="238a3-112">formato</span><span class="sxs-lookup"><span data-stu-id="238a3-112">format</span></span>     | <span data-ttu-id="238a3-113">String</span><span class="sxs-lookup"><span data-stu-id="238a3-113">String</span></span>                                     | <span data-ttu-id="238a3-114">Os valores possíveis são: `default` e `email`.</span><span class="sxs-lookup"><span data-stu-id="238a3-114">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="238a3-115">identificador</span><span class="sxs-lookup"><span data-stu-id="238a3-115">identifier</span></span> | <span data-ttu-id="238a3-116">String</span><span class="sxs-lookup"><span data-stu-id="238a3-116">String</span></span>                                     | <span data-ttu-id="238a3-117">Identificador usado para a análise de proteção de informações do Azure.</span><span class="sxs-lookup"><span data-stu-id="238a3-117">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="238a3-118">los</span><span class="sxs-lookup"><span data-stu-id="238a3-118">metadata</span></span>   | <span data-ttu-id="238a3-119">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="238a3-119">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="238a3-120">Os metadados de proteção de informações existentes da Microsoft são passados como pares chave/valor, onde a chave é o MSIP_Label_GUID_PropName.</span><span class="sxs-lookup"><span data-stu-id="238a3-120">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="238a3-121">state</span><span class="sxs-lookup"><span data-stu-id="238a3-121">state</span></span>      | <span data-ttu-id="238a3-122">String</span><span class="sxs-lookup"><span data-stu-id="238a3-122">String</span></span>                                     | <span data-ttu-id="238a3-123">Os valores possíveis são: `rest`, `motion`, `use`.</span><span class="sxs-lookup"><span data-stu-id="238a3-123">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="238a3-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="238a3-124">JSON representation</span></span>

<span data-ttu-id="238a3-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="238a3-125">The following is a JSON representation of the resource.</span></span>

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

