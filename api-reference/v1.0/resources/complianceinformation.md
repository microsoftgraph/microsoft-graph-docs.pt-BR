---
title: tipo de recurso complianceInformation
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 85fef478a8dcc0f3196355d89f0a20ef0cd7a5b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629303"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="ea41f-103">tipo de recurso complianceInformation</span><span class="sxs-lookup"><span data-stu-id="ea41f-103">complianceInformation resource type</span></span>

<span data-ttu-id="ea41f-104">Contém dados de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="ea41f-104">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="ea41f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea41f-105">Properties</span></span>

|<span data-ttu-id="ea41f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea41f-106">Property</span></span> |<span data-ttu-id="ea41f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea41f-107">Type</span></span> |<span data-ttu-id="ea41f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea41f-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="ea41f-109">certificaname</span><span class="sxs-lookup"><span data-stu-id="ea41f-109">certificationName</span></span>|<span data-ttu-id="ea41f-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea41f-110">String</span></span>| <span data-ttu-id="ea41f-111">Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="ea41f-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="ea41f-112">certificationControls</span><span class="sxs-lookup"><span data-stu-id="ea41f-112">certificationControls</span></span>|<span data-ttu-id="ea41f-113">coleção [certificationControl](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ea41f-113">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="ea41f-114">Coleção de controles de certificação associados à certificação</span><span class="sxs-lookup"><span data-stu-id="ea41f-114">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea41f-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea41f-115">JSON representation</span></span>

<span data-ttu-id="ea41f-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea41f-116">The following is a JSON representation of the resource.</span></span>

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
