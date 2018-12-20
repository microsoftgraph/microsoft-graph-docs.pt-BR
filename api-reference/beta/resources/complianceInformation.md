---
title: " tipo de recurso de complianceInformation"
description: Este recurso contém conformidade dados associados a proteger o controle de pontuação.
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380956"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="fedb9-103">tipo de recurso de complianceInformation</span><span class="sxs-lookup"><span data-stu-id="fedb9-103">complianceInformation resource type</span></span>

<span data-ttu-id="fedb9-104">Conformidade de contém dados associados a proteger o controle de pontuação.</span><span class="sxs-lookup"><span data-stu-id="fedb9-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="fedb9-105">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="fedb9-105">Property</span></span> |<span data-ttu-id="fedb9-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="fedb9-106">Type</span></span> |<span data-ttu-id="fedb9-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="fedb9-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="fedb9-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="fedb9-108">certificationName</span></span> | <span data-ttu-id="fedb9-109">string</span><span class="sxs-lookup"><span data-stu-id="fedb9-109">string</span></span> | <span data-ttu-id="fedb9-110">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="fedb9-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="fedb9-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="fedb9-111">certificationControls</span></span> | <span data-ttu-id="fedb9-112">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="fedb9-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="fedb9-113">Coleção de controles certificação associados a certificação</span><span class="sxs-lookup"><span data-stu-id="fedb9-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fedb9-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fedb9-114">JSON representation</span></span>

<span data-ttu-id="fedb9-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fedb9-115">The following is a JSON representation of the resource.</span></span>

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
