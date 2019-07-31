---
title: " tipo de recurso complianceInformation"
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b93e01bf6274591282fd5e486bebb878672d8cc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973227"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="c3220-103">tipo de recurso complianceInformation</span><span class="sxs-lookup"><span data-stu-id="c3220-103">complianceInformation resource type</span></span>

<span data-ttu-id="c3220-104">Contém dados de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="c3220-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="c3220-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3220-105">Property</span></span> |<span data-ttu-id="c3220-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3220-106">Type</span></span> |<span data-ttu-id="c3220-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3220-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="c3220-108">certificaname</span><span class="sxs-lookup"><span data-stu-id="c3220-108">certificationName</span></span> | <span data-ttu-id="c3220-109">string</span><span class="sxs-lookup"><span data-stu-id="c3220-109">string</span></span> | <span data-ttu-id="c3220-110">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="c3220-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="c3220-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="c3220-111">certificationControls</span></span> | <span data-ttu-id="c3220-112">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="c3220-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="c3220-113">Coleção de controles de certificação associados à certificação</span><span class="sxs-lookup"><span data-stu-id="c3220-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3220-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3220-114">JSON representation</span></span>

<span data-ttu-id="c3220-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3220-115">The following is a JSON representation of the resource.</span></span>

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
