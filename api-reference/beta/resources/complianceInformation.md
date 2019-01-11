---
title: " tipo de recurso de complianceInformation"
description: Este recurso contém conformidade dados associados a proteger o controle de pontuação.
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820598"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="ff2b5-103">tipo de recurso de complianceInformation</span><span class="sxs-lookup"><span data-stu-id="ff2b5-103">complianceInformation resource type</span></span>

<span data-ttu-id="ff2b5-104">Conformidade de contém dados associados a proteger o controle de pontuação.</span><span class="sxs-lookup"><span data-stu-id="ff2b5-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="ff2b5-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff2b5-105">Property</span></span> |<span data-ttu-id="ff2b5-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff2b5-106">Type</span></span> |<span data-ttu-id="ff2b5-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff2b5-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="ff2b5-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="ff2b5-108">certificationName</span></span> | <span data-ttu-id="ff2b5-109">string</span><span class="sxs-lookup"><span data-stu-id="ff2b5-109">string</span></span> | <span data-ttu-id="ff2b5-110">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="ff2b5-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="ff2b5-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="ff2b5-111">certificationControls</span></span> | <span data-ttu-id="ff2b5-112">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ff2b5-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="ff2b5-113">Coleção de controles certificação associados a certificação</span><span class="sxs-lookup"><span data-stu-id="ff2b5-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff2b5-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff2b5-114">JSON representation</span></span>

<span data-ttu-id="ff2b5-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff2b5-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
