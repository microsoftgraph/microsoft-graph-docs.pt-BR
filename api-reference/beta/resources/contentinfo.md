---
title: Tipo de recurso contentInfo
description: Representa o estado atual de algumas informações que devem ser rotuladas.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 939d7730c0de2ffb13d4dbdcade6f7c2fbce5de4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962648"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="d0da2-103">Tipo de recurso contentInfo</span><span class="sxs-lookup"><span data-stu-id="d0da2-103">contentInfo resource type</span></span>

<span data-ttu-id="d0da2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0da2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0da2-105">Representa o estado atual de algumas informações que devem ser rotuladas.</span><span class="sxs-lookup"><span data-stu-id="d0da2-105">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="d0da2-106">**contentInfo** é passado para as APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) para descrever para a API o estado atual das informações.</span><span class="sxs-lookup"><span data-stu-id="d0da2-106">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="d0da2-107">Este **detalhe contentInfo** orienta os resultados sobre quais metadados, marcação de conteúdo e proteção devem ser adicionados ou removidos quando o rótulo for aplicado, atualizado ou removido.</span><span class="sxs-lookup"><span data-stu-id="d0da2-107">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="d0da2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0da2-108">Properties</span></span>

| <span data-ttu-id="d0da2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0da2-109">Property</span></span>   | <span data-ttu-id="d0da2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0da2-110">Type</span></span>                                       | <span data-ttu-id="d0da2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0da2-111">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="d0da2-112">formato</span><span class="sxs-lookup"><span data-stu-id="d0da2-112">format</span></span>     | <span data-ttu-id="d0da2-113">String</span><span class="sxs-lookup"><span data-stu-id="d0da2-113">String</span></span>                                     | <span data-ttu-id="d0da2-114">Os valores possíveis são: `default` e `email`.</span><span class="sxs-lookup"><span data-stu-id="d0da2-114">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="d0da2-115">identificador</span><span class="sxs-lookup"><span data-stu-id="d0da2-115">identifier</span></span> | <span data-ttu-id="d0da2-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0da2-116">String</span></span>                                     | <span data-ttu-id="d0da2-117">Identificador usado para o Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="d0da2-117">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="d0da2-118">metadados</span><span class="sxs-lookup"><span data-stu-id="d0da2-118">metadata</span></span>   | <span data-ttu-id="d0da2-119">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d0da2-119">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="d0da2-120">Os metadados existentes da Proteção de Informações da Microsoft são passados como pares de chave/valor, onde a chave é a MSIP_Label_GUID_PropName.</span><span class="sxs-lookup"><span data-stu-id="d0da2-120">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="d0da2-121">estado</span><span class="sxs-lookup"><span data-stu-id="d0da2-121">state</span></span>      | <span data-ttu-id="d0da2-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0da2-122">String</span></span>                                     | <span data-ttu-id="d0da2-123">Os valores possíveis são: `rest`, `motion`, `use`.</span><span class="sxs-lookup"><span data-stu-id="d0da2-123">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="d0da2-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0da2-124">JSON representation</span></span>

<span data-ttu-id="d0da2-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0da2-125">The following is a JSON representation of the resource.</span></span>

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

