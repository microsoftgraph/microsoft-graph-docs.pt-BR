---
title: tipo de recurso downgradeJustification
description: Representa a entrada do usuário sobre por que o downgrade foi realizado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aacc32ac86df4eda087f49dbb3dca05a356e8080
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939422"
---
# <a name="downgradejustification-resource-type"></a><span data-ttu-id="57814-103">tipo de recurso downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="57814-103">downgradeJustification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57814-104">Representa a entrada do usuário sobre por que o downgrade foi realizado.</span><span class="sxs-lookup"><span data-stu-id="57814-104">Represents user input on why downgrade was performed.</span></span> <span data-ttu-id="57814-105">A justificação de downgrade pode ser necessária com base na configuração de política de rótulo no centro de conformidade e segurança do Office.</span><span class="sxs-lookup"><span data-stu-id="57814-105">Downgrade justification might be required based on label policy configuration in Office Security and Compliance Center.</span></span>

## <a name="properties"></a><span data-ttu-id="57814-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57814-106">Properties</span></span>

| <span data-ttu-id="57814-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57814-107">Property</span></span>             | <span data-ttu-id="57814-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="57814-108">Type</span></span>    | <span data-ttu-id="57814-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="57814-109">Description</span></span>                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="57814-110">isDowngradeJustified</span><span class="sxs-lookup"><span data-stu-id="57814-110">isDowngradeJustified</span></span> | <span data-ttu-id="57814-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="57814-111">Boolean</span></span> | <span data-ttu-id="57814-112">Indica se o downgrade é ou não justificado.</span><span class="sxs-lookup"><span data-stu-id="57814-112">Indicates whether the downgrade is or is not justified.</span></span>                                              |
| <span data-ttu-id="57814-113">justificationMessage</span><span class="sxs-lookup"><span data-stu-id="57814-113">justificationMessage</span></span> | <span data-ttu-id="57814-114">String</span><span class="sxs-lookup"><span data-stu-id="57814-114">String</span></span>  | <span data-ttu-id="57814-115">Mensagem que indica por que um downgrade é justificado.</span><span class="sxs-lookup"><span data-stu-id="57814-115">Message that indicates why a downgrade is justified.</span></span> <span data-ttu-id="57814-116">A mensagem aparecerá em logs administrativos.</span><span class="sxs-lookup"><span data-stu-id="57814-116">The message will appear in administrative logs.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57814-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57814-117">JSON representation</span></span>

<span data-ttu-id="57814-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57814-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.downgradeJustification",
  "baseType": null
}-->

```json
{
  "isDowngradeJustified": true,
  "justificationMessage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "downgradeJustification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->