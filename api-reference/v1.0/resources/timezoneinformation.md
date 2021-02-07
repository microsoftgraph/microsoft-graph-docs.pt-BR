---
title: Tipo de recurso timeZoneInformation
description: Representa um fuso horário. O formato suportado é o Windows e o fuso horário IANA (autoridade de números atribuídos à Internet) (também conhecido como fuso horário de Olson)
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 146ea2e965368a7b025a83038e7377e6379bf4a2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136630"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="8977c-104">Tipo de recurso timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="8977c-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="8977c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8977c-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="8977c-106">Representa um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8977c-106">Represents a time zone.</span></span> <span data-ttu-id="8977c-107">Entre os formatos de fuso horário válidos estão o do Windows e o da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson), além de quando o atual problema conhecido foi corrigido.</span><span class="sxs-lookup"><span data-stu-id="8977c-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="8977c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8977c-108">Properties</span></span>
| <span data-ttu-id="8977c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8977c-109">Property</span></span>     | <span data-ttu-id="8977c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8977c-110">Type</span></span>   |<span data-ttu-id="8977c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8977c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8977c-112">alias</span><span class="sxs-lookup"><span data-stu-id="8977c-112">alias</span></span>|<span data-ttu-id="8977c-113">string</span><span class="sxs-lookup"><span data-stu-id="8977c-113">string</span></span>|<span data-ttu-id="8977c-114">Um identificador para o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8977c-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="8977c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8977c-115">displayName</span></span>|<span data-ttu-id="8977c-116">string</span><span class="sxs-lookup"><span data-stu-id="8977c-116">string</span></span>|<span data-ttu-id="8977c-117">Uma sequência de caracteres de exibição que representa o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8977c-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8977c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8977c-118">JSON representation</span></span>

<span data-ttu-id="8977c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8977c-119">Here is a JSON representation of the resource.</span></span>

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

