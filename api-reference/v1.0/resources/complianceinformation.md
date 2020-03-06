---
title: tipo de recurso complianceInformation
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ef62f6df73c24f9e6b3884921865c28ea152a3dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533033"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="e711f-103">tipo de recurso complianceInformation</span><span class="sxs-lookup"><span data-stu-id="e711f-103">complianceInformation resource type</span></span>

<span data-ttu-id="e711f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e711f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e711f-105">Contém dados de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="e711f-105">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="e711f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e711f-106">Properties</span></span>

|<span data-ttu-id="e711f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e711f-107">Property</span></span> |<span data-ttu-id="e711f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e711f-108">Type</span></span> |<span data-ttu-id="e711f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e711f-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="e711f-110">certificaname</span><span class="sxs-lookup"><span data-stu-id="e711f-110">certificationName</span></span>|<span data-ttu-id="e711f-111">String</span><span class="sxs-lookup"><span data-stu-id="e711f-111">String</span></span>| <span data-ttu-id="e711f-112">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="e711f-112">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="e711f-113">certificationControls</span><span class="sxs-lookup"><span data-stu-id="e711f-113">certificationControls</span></span>|<span data-ttu-id="e711f-114">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="e711f-114">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="e711f-115">Coleção de controles de certificação associados à certificação</span><span class="sxs-lookup"><span data-stu-id="e711f-115">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e711f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e711f-116">JSON representation</span></span>

<span data-ttu-id="e711f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e711f-117">The following is a JSON representation of the resource.</span></span>

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
