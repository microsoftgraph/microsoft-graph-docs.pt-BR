---
title: tipo de recurso recommendLabelAction
description: Representa um rótulo que deve ser recomendado para o usuário para o aplicativo para o arquivo com base em tipos de informações confidenciais.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f2a872c0aa64eb79e0b8755ddc6b3788f14055
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939373"
---
# <a name="recommendlabelaction-resource-type"></a><span data-ttu-id="25843-103">tipo de recurso recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="25843-103">recommendLabelAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25843-104">Representa um rótulo que deve ser recomendado para o usuário para o aplicativo no arquivo com base em tipos de informações confidenciais descobertos.</span><span class="sxs-lookup"><span data-stu-id="25843-104">Represents a label that should be recommended to the user for application to the file based on discovered sensitive information types.</span></span> <span data-ttu-id="25843-105">O [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) poderá retornar um **recommendLabelAction** se a política de rótulo de proteção de informações da Microsoft estiver definida como **recomendar** e rotular em vez de impor um rótulo.</span><span class="sxs-lookup"><span data-stu-id="25843-105">The [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) may return a **recommendLabelAction** if the Microsoft Information Protection labeling policy is set to **recommend** and label rather than enforce a label.</span></span> <span data-ttu-id="25843-106">O usuário ou a aplicação pode optar por ignorar ou aceitar a recomendação.</span><span class="sxs-lookup"><span data-stu-id="25843-106">The user or appliation may choose to ignore or accept the recommendation.</span></span> 

## <a name="properties"></a><span data-ttu-id="25843-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25843-107">Properties</span></span>

| <span data-ttu-id="25843-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25843-108">Property</span></span>                    | <span data-ttu-id="25843-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="25843-109">Type</span></span>                                                                     | <span data-ttu-id="25843-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="25843-110">Description</span></span>                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="25843-111">ação</span><span class="sxs-lookup"><span data-stu-id="25843-111">actionSource</span></span>                | <span data-ttu-id="25843-112">String</span><span class="sxs-lookup"><span data-stu-id="25843-112">String</span></span>                                                                   | <span data-ttu-id="25843-113">Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="25843-113">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span> |
| <span data-ttu-id="25843-114">actions</span><span class="sxs-lookup"><span data-stu-id="25843-114">actions</span></span>                     | <span data-ttu-id="25843-115">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="25843-115">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="25843-116">Ações a serem executadas se o rótulo for aceito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="25843-116">Actions to take if the label is accepted by the user.</span></span>                                                                       |
| <span data-ttu-id="25843-117">rótulo</span><span class="sxs-lookup"><span data-stu-id="25843-117">label</span></span>                       | [<span data-ttu-id="25843-118">labelDetails</span><span class="sxs-lookup"><span data-stu-id="25843-118">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="25843-119">O rótulo que está sendo recomendado.</span><span class="sxs-lookup"><span data-stu-id="25843-119">The label that is being recommended.</span></span>                                                                      |
| <span data-ttu-id="25843-120">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="25843-120">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="25843-121">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="25843-121">Guid collection</span></span>                                                          | <span data-ttu-id="25843-122">Os GUIDs de tipo de informações confidenciais que causaram a recomendação para serem fornecidos.</span><span class="sxs-lookup"><span data-stu-id="25843-122">The sensitive information type GUIDs that caused the recommendation to be given.</span></span>                                                                      |

## <a name="json-representation"></a><span data-ttu-id="25843-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25843-123">JSON representation</span></span>

<span data-ttu-id="25843-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25843-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recommendLabelAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "actionSource": "String",
  "actions": [{"@odata.type": "microsoft.graph.informationProtectionAction"}],
  "label": {"@odata.type": "microsoft.graph.labelDetails"},
  "responsibleSensitiveTypeIds": ["Guid"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recommendLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
