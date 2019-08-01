---
title: tipo de recurso complianceInformation
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9fc47940b8a9f249e66092ee016453a9eb5152ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032855"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="59cf1-103">tipo de recurso complianceInformation</span><span class="sxs-lookup"><span data-stu-id="59cf1-103">complianceInformation resource type</span></span>

<span data-ttu-id="59cf1-104">Contém dados de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="59cf1-104">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="59cf1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59cf1-105">Properties</span></span>

|<span data-ttu-id="59cf1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59cf1-106">Property</span></span> |<span data-ttu-id="59cf1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="59cf1-107">Type</span></span> |<span data-ttu-id="59cf1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="59cf1-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="59cf1-109">certificaname</span><span class="sxs-lookup"><span data-stu-id="59cf1-109">certificationName</span></span>|<span data-ttu-id="59cf1-110">String</span><span class="sxs-lookup"><span data-stu-id="59cf1-110">String</span></span>| <span data-ttu-id="59cf1-111">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="59cf1-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="59cf1-112">certificationControls</span><span class="sxs-lookup"><span data-stu-id="59cf1-112">certificationControls</span></span>|<span data-ttu-id="59cf1-113">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="59cf1-113">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="59cf1-114">Coleção de controles de certificação associados à certificação</span><span class="sxs-lookup"><span data-stu-id="59cf1-114">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59cf1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59cf1-115">JSON representation</span></span>

<span data-ttu-id="59cf1-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59cf1-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": [{"@odata.type": "microsoft.graph.certificationControl"}]
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
