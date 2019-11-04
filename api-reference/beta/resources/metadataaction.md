---
title: tipo de recurso metadataaction
description: Representa os metadados a serem gravados ou removidos de um arquivo.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8652a33de04d0a28a34c3738dd1706d6aff5e5b9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938902"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="d2b1b-103">tipo de recurso metadataaction</span><span class="sxs-lookup"><span data-stu-id="d2b1b-103">metadataAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2b1b-104">Representa os metadados a serem gravados ou removidos de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="d2b1b-104">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="d2b1b-105">**metadataaction** pode ser retornado pelas APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) .</span><span class="sxs-lookup"><span data-stu-id="d2b1b-105">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="d2b1b-106">A ação informa o aplicativo de consumo dos pares chave/valor específicos que devem ser adicionados ao arquivo ou as chaves de metadados específicas que devem ser removidas do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d2b1b-106">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="d2b1b-107">Este metadados é o que descreve o arquivo ou as informações que estão sendo *rotuladas*.</span><span class="sxs-lookup"><span data-stu-id="d2b1b-107">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="d2b1b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2b1b-108">Properties</span></span>

| <span data-ttu-id="d2b1b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2b1b-109">Property</span></span>         | <span data-ttu-id="d2b1b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2b1b-110">Type</span></span>                                       | <span data-ttu-id="d2b1b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2b1b-111">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="d2b1b-112">metadataToAdd</span><span class="sxs-lookup"><span data-stu-id="d2b1b-112">metadataToAdd</span></span>    | <span data-ttu-id="d2b1b-113">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d2b1b-113">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="d2b1b-114">Uma coleção de pares chave de valor que deve ser adicionado ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="d2b1b-114">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="d2b1b-115">metadataToRemove</span><span class="sxs-lookup"><span data-stu-id="d2b1b-115">metadataToRemove</span></span> | <span data-ttu-id="d2b1b-116">String collection</span><span class="sxs-lookup"><span data-stu-id="d2b1b-116">String collection</span></span>                          | <span data-ttu-id="d2b1b-117">Uma coleção de cadeias de caracteres que indicam quais teclas serão removidas dos metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d2b1b-117">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d2b1b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2b1b-118">JSON representation</span></span>

<span data-ttu-id="d2b1b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2b1b-119">The following is a JSON representation of the resource.</span></span>

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