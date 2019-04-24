---
title: Tipo de recurso timeZoneInformation
description: Representa um fuso horário. O formato com suporte é Windows e o fuso horário da autoridade de números atribuídos pela Internet (IANA) (também conhecido como fuso horário Olson)
localization_priority: Normal
ms.openlocfilehash: ced18a28a5c086416fa7247e1531d772fd63b977
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456910"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="47e87-104">Tipo de recurso timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="47e87-104">timeZoneInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47e87-105">Representa um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="47e87-105">Represents a time zone.</span></span> <span data-ttu-id="47e87-106">Entre os formatos de fuso horário válidos estão o do Windows e o da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson), além de quando o atual problema conhecido foi corrigido.</span><span class="sxs-lookup"><span data-stu-id="47e87-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="47e87-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47e87-107">Properties</span></span>
| <span data-ttu-id="47e87-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47e87-108">Property</span></span>     | <span data-ttu-id="47e87-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="47e87-109">Type</span></span>   |<span data-ttu-id="47e87-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="47e87-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47e87-111">alias</span><span class="sxs-lookup"><span data-stu-id="47e87-111">alias</span></span>|<span data-ttu-id="47e87-112">string</span><span class="sxs-lookup"><span data-stu-id="47e87-112">string</span></span>|<span data-ttu-id="47e87-113">Um identificador para o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="47e87-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="47e87-114">displayName</span><span class="sxs-lookup"><span data-stu-id="47e87-114">displayName</span></span>|<span data-ttu-id="47e87-115">string</span><span class="sxs-lookup"><span data-stu-id="47e87-115">string</span></span>|<span data-ttu-id="47e87-116">Uma sequência de caracteres de exibição que representa o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="47e87-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47e87-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47e87-117">JSON representation</span></span>

<span data-ttu-id="47e87-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47e87-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timezoneinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
