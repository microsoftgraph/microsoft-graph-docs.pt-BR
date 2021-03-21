---
title: Tipo de recurso metadataAction
description: Representa os metadados a serem gravados ou removidos de um arquivo.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 23305d8a3e1e89d198b4700e794dd264eabf003b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960394"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="dda3d-103">Tipo de recurso metadataAction</span><span class="sxs-lookup"><span data-stu-id="dda3d-103">metadataAction resource type</span></span>

<span data-ttu-id="dda3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dda3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dda3d-105">Representa os metadados a serem gravados ou removidos de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="dda3d-105">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="dda3d-106">**metadataAction** pode ser retornada pelas APIs [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [evaluateClassificationResults.](../api/informationprotectionlabel-evaluateclassificationresults.md)</span><span class="sxs-lookup"><span data-stu-id="dda3d-106">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="dda3d-107">A ação informa o aplicativo de consumo dos pares de chave/valor específicos que devem ser adicionados ao arquivo ou às chaves de metadados específicas que devem ser removidas do arquivo.</span><span class="sxs-lookup"><span data-stu-id="dda3d-107">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="dda3d-108">Esse metadados é o que descreve o arquivo ou informações como *sendo rotulados*.</span><span class="sxs-lookup"><span data-stu-id="dda3d-108">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="dda3d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dda3d-109">Properties</span></span>

| <span data-ttu-id="dda3d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dda3d-110">Property</span></span>         | <span data-ttu-id="dda3d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dda3d-111">Type</span></span>                                       | <span data-ttu-id="dda3d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dda3d-112">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="dda3d-113">metadataToAdd</span><span class="sxs-lookup"><span data-stu-id="dda3d-113">metadataToAdd</span></span>    | <span data-ttu-id="dda3d-114">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="dda3d-114">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="dda3d-115">Uma coleção de pares de valores-chave que devem ser adicionados ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="dda3d-115">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="dda3d-116">metadataToRemove</span><span class="sxs-lookup"><span data-stu-id="dda3d-116">metadataToRemove</span></span> | <span data-ttu-id="dda3d-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dda3d-117">String collection</span></span>                          | <span data-ttu-id="dda3d-118">Uma coleção de cadeias de caracteres que indica quais chaves remover dos metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="dda3d-118">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dda3d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dda3d-119">JSON representation</span></span>

<span data-ttu-id="dda3d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dda3d-120">The following is a JSON representation of the resource.</span></span>

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

