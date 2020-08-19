---
title: Tipo de recurso timeZoneInformation
description: Representa um fuso horário. O formato com suporte é Windows e o fuso horário da autoridade de números atribuídos pela Internet (IANA) (também conhecido como fuso horário Olson)
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 81f1eb3f8abbdcf95b94407019807d0d002dc286
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811823"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="380ab-104">Tipo de recurso timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="380ab-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="380ab-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="380ab-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="380ab-106">Representa um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="380ab-106">Represents a time zone.</span></span> <span data-ttu-id="380ab-107">Entre os formatos de fuso horário válidos estão o do Windows e o da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson), além de quando o atual problema conhecido foi corrigido.</span><span class="sxs-lookup"><span data-stu-id="380ab-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="380ab-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="380ab-108">Properties</span></span>
| <span data-ttu-id="380ab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="380ab-109">Property</span></span>     | <span data-ttu-id="380ab-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="380ab-110">Type</span></span>   |<span data-ttu-id="380ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="380ab-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="380ab-112">alias</span><span class="sxs-lookup"><span data-stu-id="380ab-112">alias</span></span>|<span data-ttu-id="380ab-113">string</span><span class="sxs-lookup"><span data-stu-id="380ab-113">string</span></span>|<span data-ttu-id="380ab-114">Um identificador para o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="380ab-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="380ab-115">displayName</span><span class="sxs-lookup"><span data-stu-id="380ab-115">displayName</span></span>|<span data-ttu-id="380ab-116">string</span><span class="sxs-lookup"><span data-stu-id="380ab-116">string</span></span>|<span data-ttu-id="380ab-117">Uma sequência de caracteres de exibição que representa o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="380ab-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="380ab-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="380ab-118">JSON representation</span></span>

<span data-ttu-id="380ab-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="380ab-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
