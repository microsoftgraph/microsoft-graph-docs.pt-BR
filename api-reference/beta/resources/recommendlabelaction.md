---
title: tipo de recurso recommendLabelAction
description: Representa um rótulo que deve ser recomendado para o usuário para o aplicativo para o arquivo com base em tipos de informações confidenciais.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b5deebaec460bd8c1993cc0c308e68e6f6f986a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055180"
---
# <a name="recommendlabelaction-resource-type"></a><span data-ttu-id="88ea3-103">tipo de recurso recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="88ea3-103">recommendLabelAction resource type</span></span>

<span data-ttu-id="88ea3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ea3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88ea3-105">Representa um rótulo que deve ser recomendado para o usuário para o aplicativo no arquivo com base em tipos de informações confidenciais descobertos.</span><span class="sxs-lookup"><span data-stu-id="88ea3-105">Represents a label that should be recommended to the user for application to the file based on discovered sensitive information types.</span></span> <span data-ttu-id="88ea3-106">O [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) poderá retornar um **recommendLabelAction** se a política de rótulo de proteção de informações da Microsoft estiver definida como **recomendar** e rotular em vez de impor um rótulo.</span><span class="sxs-lookup"><span data-stu-id="88ea3-106">The [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) may return a **recommendLabelAction** if the Microsoft Information Protection labeling policy is set to **recommend** and label rather than enforce a label.</span></span> <span data-ttu-id="88ea3-107">O usuário ou a aplicação pode optar por ignorar ou aceitar a recomendação.</span><span class="sxs-lookup"><span data-stu-id="88ea3-107">The user or appliation may choose to ignore or accept the recommendation.</span></span> 

## <a name="properties"></a><span data-ttu-id="88ea3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88ea3-108">Properties</span></span>

| <span data-ttu-id="88ea3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88ea3-109">Property</span></span>                    | <span data-ttu-id="88ea3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="88ea3-110">Type</span></span>                                                                     | <span data-ttu-id="88ea3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="88ea3-111">Description</span></span>                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="88ea3-112">ação</span><span class="sxs-lookup"><span data-stu-id="88ea3-112">actionSource</span></span>                | <span data-ttu-id="88ea3-113">String</span><span class="sxs-lookup"><span data-stu-id="88ea3-113">String</span></span>                                                                   | <span data-ttu-id="88ea3-114">Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`.</span><span class="sxs-lookup"><span data-stu-id="88ea3-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span> |
| <span data-ttu-id="88ea3-115">actions</span><span class="sxs-lookup"><span data-stu-id="88ea3-115">actions</span></span>                     | <span data-ttu-id="88ea3-116">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="88ea3-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="88ea3-117">Ações a serem executadas se o rótulo for aceito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="88ea3-117">Actions to take if the label is accepted by the user.</span></span>                                                                       |
| <span data-ttu-id="88ea3-118">rótulo</span><span class="sxs-lookup"><span data-stu-id="88ea3-118">label</span></span>                       | [<span data-ttu-id="88ea3-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="88ea3-119">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="88ea3-120">O rótulo que está sendo recomendado.</span><span class="sxs-lookup"><span data-stu-id="88ea3-120">The label that is being recommended.</span></span>                                                                      |
| <span data-ttu-id="88ea3-121">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="88ea3-121">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="88ea3-122">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="88ea3-122">Guid collection</span></span>                                                          | <span data-ttu-id="88ea3-123">Os GUIDs de tipo de informações confidenciais que causaram a recomendação para serem fornecidos.</span><span class="sxs-lookup"><span data-stu-id="88ea3-123">The sensitive information type GUIDs that caused the recommendation to be given.</span></span>                                                                      |

## <a name="json-representation"></a><span data-ttu-id="88ea3-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88ea3-124">JSON representation</span></span>

<span data-ttu-id="88ea3-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88ea3-125">The following is a JSON representation of the resource.</span></span>

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


