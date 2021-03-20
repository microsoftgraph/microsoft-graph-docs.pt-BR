---
title: Tipo de recurso downgradeJustification
description: Representa a entrada do usuário sobre por que a rebaixamento foi realizada.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: bc7336469f93de9e6d2b07fe73df9dce2eafd47f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941796"
---
# <a name="downgradejustification-resource-type"></a><span data-ttu-id="7b04c-103">Tipo de recurso downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="7b04c-103">downgradeJustification resource type</span></span>

<span data-ttu-id="7b04c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b04c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b04c-105">Representa a entrada do usuário sobre por que a rebaixamento foi realizada.</span><span class="sxs-lookup"><span data-stu-id="7b04c-105">Represents user input on why downgrade was performed.</span></span> <span data-ttu-id="7b04c-106">A justificativa de downgrade pode ser necessária com base na configuração da política de rótulo no Centro de Conformidade e Segurança do Office.</span><span class="sxs-lookup"><span data-stu-id="7b04c-106">Downgrade justification might be required based on label policy configuration in Office Security and Compliance Center.</span></span>

## <a name="properties"></a><span data-ttu-id="7b04c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b04c-107">Properties</span></span>

| <span data-ttu-id="7b04c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b04c-108">Property</span></span>             | <span data-ttu-id="7b04c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b04c-109">Type</span></span>    | <span data-ttu-id="7b04c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b04c-110">Description</span></span>                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7b04c-111">isDowngradeJustified</span><span class="sxs-lookup"><span data-stu-id="7b04c-111">isDowngradeJustified</span></span> | <span data-ttu-id="7b04c-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b04c-112">Boolean</span></span> | <span data-ttu-id="7b04c-113">Indica se a rebaixamento é ou não justificada.</span><span class="sxs-lookup"><span data-stu-id="7b04c-113">Indicates whether the downgrade is or is not justified.</span></span>                                              |
| <span data-ttu-id="7b04c-114">justificationMessage</span><span class="sxs-lookup"><span data-stu-id="7b04c-114">justificationMessage</span></span> | <span data-ttu-id="7b04c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b04c-115">String</span></span>  | <span data-ttu-id="7b04c-116">Mensagem que indica por que uma rebaixamento é justificada.</span><span class="sxs-lookup"><span data-stu-id="7b04c-116">Message that indicates why a downgrade is justified.</span></span> <span data-ttu-id="7b04c-117">A mensagem aparecerá em logs administrativos.</span><span class="sxs-lookup"><span data-stu-id="7b04c-117">The message will appear in administrative logs.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b04c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b04c-118">JSON representation</span></span>

<span data-ttu-id="7b04c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b04c-119">The following is a JSON representation of the resource.</span></span>

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

