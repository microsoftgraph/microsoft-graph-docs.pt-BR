---
title: " tipo de recurso complianceInformation"
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 65eda1c24fee112ef18fc6682b537f92f924dcf8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507573"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="d3546-103">tipo de recurso complianceInformation</span><span class="sxs-lookup"><span data-stu-id="d3546-103">complianceInformation resource type</span></span>

<span data-ttu-id="d3546-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3546-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3546-105">Contém dados de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="d3546-105">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="d3546-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3546-106">Property</span></span> |<span data-ttu-id="d3546-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3546-107">Type</span></span> |<span data-ttu-id="d3546-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3546-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="d3546-109">certificaname</span><span class="sxs-lookup"><span data-stu-id="d3546-109">certificationName</span></span> | <span data-ttu-id="d3546-110">string</span><span class="sxs-lookup"><span data-stu-id="d3546-110">string</span></span> | <span data-ttu-id="d3546-111">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="d3546-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="d3546-112">certificationControls</span><span class="sxs-lookup"><span data-stu-id="d3546-112">certificationControls</span></span> | <span data-ttu-id="d3546-113">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="d3546-113">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="d3546-114">Coleção de controles de certificação associados à certificação</span><span class="sxs-lookup"><span data-stu-id="d3546-114">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3546-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3546-115">JSON representation</span></span>

<span data-ttu-id="d3546-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3546-116">The following is a JSON representation of the resource.</span></span>

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
