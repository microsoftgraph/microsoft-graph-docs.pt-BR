---
title: " tipo de recurso complianceInformation"
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543361"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="5deff-103">tipo de recurso complianceInformation</span><span class="sxs-lookup"><span data-stu-id="5deff-103">complianceInformation resource type</span></span>

<span data-ttu-id="5deff-104">Contém dados de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="5deff-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="5deff-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5deff-105">Property</span></span> |<span data-ttu-id="5deff-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="5deff-106">Type</span></span> |<span data-ttu-id="5deff-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="5deff-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="5deff-108">certificaname</span><span class="sxs-lookup"><span data-stu-id="5deff-108">certificationName</span></span> | <span data-ttu-id="5deff-109">string</span><span class="sxs-lookup"><span data-stu-id="5deff-109">string</span></span> | <span data-ttu-id="5deff-110">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="5deff-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="5deff-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="5deff-111">certificationControls</span></span> | <span data-ttu-id="5deff-112">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="5deff-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="5deff-113">Coleção de controles de certificação associados à certificação</span><span class="sxs-lookup"><span data-stu-id="5deff-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5deff-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5deff-114">JSON representation</span></span>

<span data-ttu-id="5deff-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5deff-115">The following is a JSON representation of the resource.</span></span>

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
