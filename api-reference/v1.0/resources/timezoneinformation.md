---
title: Tipo de recurso timeZoneInformation
description: Representa um fuso horário. O formato com suporte é Windows e Internet Assigned Numbers Authority (IANA) hora (também conhecido como fuso horário Olson) de zona
ms.openlocfilehash: de80ed293af834d299be5f9543c5c3bedde7a540
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003526"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="b0009-104">Tipo de recurso timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="b0009-104">timeZoneInformation resource type</span></span>


<span data-ttu-id="b0009-105">Representa um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b0009-105">Represents a time zone.</span></span> <span data-ttu-id="b0009-106">Entre os formatos de fuso horário válidos estão o do Windows e o da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson), além de quando o atual problema conhecido foi corrigido.</span><span class="sxs-lookup"><span data-stu-id="b0009-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="b0009-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0009-107">Properties</span></span>
| <span data-ttu-id="b0009-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0009-108">Property</span></span>     | <span data-ttu-id="b0009-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0009-109">Type</span></span>   |<span data-ttu-id="b0009-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0009-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0009-111">alias</span><span class="sxs-lookup"><span data-stu-id="b0009-111">alias</span></span>|<span data-ttu-id="b0009-112">string</span><span class="sxs-lookup"><span data-stu-id="b0009-112">string</span></span>|<span data-ttu-id="b0009-113">Um identificador para o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b0009-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="b0009-114">displayName</span><span class="sxs-lookup"><span data-stu-id="b0009-114">displayName</span></span>|<span data-ttu-id="b0009-115">string</span><span class="sxs-lookup"><span data-stu-id="b0009-115">string</span></span>|<span data-ttu-id="b0009-116">Uma sequência de caracteres de exibição que representa o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b0009-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0009-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0009-117">JSON representation</span></span>

<span data-ttu-id="b0009-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0009-118">Here is a JSON representation of the resource.</span></span>

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