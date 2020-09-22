---
title: tipo de recurso complianceInformation
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 00447f134b2c54bdda92857c6c84c05e8c52b3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018932"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="3be55-103">tipo de recurso complianceInformation</span><span class="sxs-lookup"><span data-stu-id="3be55-103">complianceInformation resource type</span></span>

<span data-ttu-id="3be55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3be55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3be55-105">Contém dados de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="3be55-105">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="3be55-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3be55-106">Properties</span></span>

|<span data-ttu-id="3be55-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3be55-107">Property</span></span> |<span data-ttu-id="3be55-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be55-108">Type</span></span> |<span data-ttu-id="3be55-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be55-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="3be55-110">certificaname</span><span class="sxs-lookup"><span data-stu-id="3be55-110">certificationName</span></span>|<span data-ttu-id="3be55-111">String</span><span class="sxs-lookup"><span data-stu-id="3be55-111">String</span></span>| <span data-ttu-id="3be55-112">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="3be55-112">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="3be55-113">certificationControls</span><span class="sxs-lookup"><span data-stu-id="3be55-113">certificationControls</span></span>|<span data-ttu-id="3be55-114">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="3be55-114">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="3be55-115">Coleção de controles de certificação associados à certificação</span><span class="sxs-lookup"><span data-stu-id="3be55-115">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3be55-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3be55-116">JSON representation</span></span>

<span data-ttu-id="3be55-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3be55-117">The following is a JSON representation of the resource.</span></span>

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

