---
title: tipo de recurso metadataaction
description: Representa os metadados a serem gravados ou removidos de um arquivo.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55ddd644428662f6a646fd9c003761ab6f7c1e9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021382"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="1d5da-103">tipo de recurso metadataaction</span><span class="sxs-lookup"><span data-stu-id="1d5da-103">metadataAction resource type</span></span>

<span data-ttu-id="1d5da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d5da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d5da-105">Representa os metadados a serem gravados ou removidos de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="1d5da-105">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="1d5da-106">**metadataaction** pode ser retornado pelas APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) .</span><span class="sxs-lookup"><span data-stu-id="1d5da-106">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="1d5da-107">A ação informa o aplicativo de consumo dos pares chave/valor específicos que devem ser adicionados ao arquivo ou as chaves de metadados específicas que devem ser removidas do arquivo.</span><span class="sxs-lookup"><span data-stu-id="1d5da-107">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="1d5da-108">Este metadados é o que descreve o arquivo ou as informações que estão sendo *rotuladas*.</span><span class="sxs-lookup"><span data-stu-id="1d5da-108">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="1d5da-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d5da-109">Properties</span></span>

| <span data-ttu-id="1d5da-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d5da-110">Property</span></span>         | <span data-ttu-id="1d5da-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d5da-111">Type</span></span>                                       | <span data-ttu-id="1d5da-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d5da-112">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="1d5da-113">metadataToAdd</span><span class="sxs-lookup"><span data-stu-id="1d5da-113">metadataToAdd</span></span>    | <span data-ttu-id="1d5da-114">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1d5da-114">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="1d5da-115">Uma coleção de pares chave de valor que deve ser adicionado ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="1d5da-115">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="1d5da-116">metadataToRemove</span><span class="sxs-lookup"><span data-stu-id="1d5da-116">metadataToRemove</span></span> | <span data-ttu-id="1d5da-117">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1d5da-117">String collection</span></span>                          | <span data-ttu-id="1d5da-118">Uma coleção de cadeias de caracteres que indicam quais teclas serão removidas dos metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="1d5da-118">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1d5da-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d5da-119">JSON representation</span></span>

<span data-ttu-id="1d5da-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d5da-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "metadataToAdd": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "metadataToRemove": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

