---
title: tipo de recurso downgradeJustification
description: Representa a entrada do usuário sobre por que o downgrade foi realizado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91bcb5a8e12a159bf2c6586a0e3dc49a540a69f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505788"
---
# <a name="downgradejustification-resource-type"></a><span data-ttu-id="1892b-103">tipo de recurso downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="1892b-103">downgradeJustification resource type</span></span>

<span data-ttu-id="1892b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1892b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1892b-105">Representa a entrada do usuário sobre por que o downgrade foi realizado.</span><span class="sxs-lookup"><span data-stu-id="1892b-105">Represents user input on why downgrade was performed.</span></span> <span data-ttu-id="1892b-106">A justificação de downgrade pode ser necessária com base na configuração de política de rótulo no centro de conformidade e segurança do Office.</span><span class="sxs-lookup"><span data-stu-id="1892b-106">Downgrade justification might be required based on label policy configuration in Office Security and Compliance Center.</span></span>

## <a name="properties"></a><span data-ttu-id="1892b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1892b-107">Properties</span></span>

| <span data-ttu-id="1892b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1892b-108">Property</span></span>             | <span data-ttu-id="1892b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1892b-109">Type</span></span>    | <span data-ttu-id="1892b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1892b-110">Description</span></span>                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1892b-111">isDowngradeJustified</span><span class="sxs-lookup"><span data-stu-id="1892b-111">isDowngradeJustified</span></span> | <span data-ttu-id="1892b-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="1892b-112">Boolean</span></span> | <span data-ttu-id="1892b-113">Indica se o downgrade é ou não justificado.</span><span class="sxs-lookup"><span data-stu-id="1892b-113">Indicates whether the downgrade is or is not justified.</span></span>                                              |
| <span data-ttu-id="1892b-114">justificationMessage</span><span class="sxs-lookup"><span data-stu-id="1892b-114">justificationMessage</span></span> | <span data-ttu-id="1892b-115">String</span><span class="sxs-lookup"><span data-stu-id="1892b-115">String</span></span>  | <span data-ttu-id="1892b-116">Mensagem que indica por que um downgrade é justificado.</span><span class="sxs-lookup"><span data-stu-id="1892b-116">Message that indicates why a downgrade is justified.</span></span> <span data-ttu-id="1892b-117">A mensagem aparecerá em logs administrativos.</span><span class="sxs-lookup"><span data-stu-id="1892b-117">The message will appear in administrative logs.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1892b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1892b-118">JSON representation</span></span>

<span data-ttu-id="1892b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1892b-119">The following is a JSON representation of the resource.</span></span>

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