---
title: Tipo de recurso timeZoneInformation
description: Representa um fuso horário. O formato com suporte é Windows e Internet Assigned Numbers Authority (IANA) hora (também conhecido como fuso horário Olson) de zona
ms.openlocfilehash: 5508f20812b8327a068364df7eb33c5072c3512e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036669"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="bc26d-104">Tipo de recurso timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="bc26d-104">timeZoneInformation resource type</span></span>

> <span data-ttu-id="bc26d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bc26d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc26d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bc26d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc26d-107">Representa um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="bc26d-107">Represents a time zone.</span></span> <span data-ttu-id="bc26d-108">Entre os formatos de fuso horário válidos estão o do Windows e o da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson), além de quando o atual problema conhecido foi corrigido.</span><span class="sxs-lookup"><span data-stu-id="bc26d-108">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="bc26d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc26d-109">Properties</span></span>
| <span data-ttu-id="bc26d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc26d-110">Property</span></span>     | <span data-ttu-id="bc26d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc26d-111">Type</span></span>   |<span data-ttu-id="bc26d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc26d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc26d-113">alias</span><span class="sxs-lookup"><span data-stu-id="bc26d-113">alias</span></span>|<span data-ttu-id="bc26d-114">string</span><span class="sxs-lookup"><span data-stu-id="bc26d-114">string</span></span>|<span data-ttu-id="bc26d-115">Um identificador para o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="bc26d-115">An identifier for the time zone.</span></span>|
|<span data-ttu-id="bc26d-116">displayName</span><span class="sxs-lookup"><span data-stu-id="bc26d-116">displayName</span></span>|<span data-ttu-id="bc26d-117">string</span><span class="sxs-lookup"><span data-stu-id="bc26d-117">string</span></span>|<span data-ttu-id="bc26d-118">Uma sequência de caracteres de exibição que representa o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="bc26d-118">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc26d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc26d-119">JSON representation</span></span>

<span data-ttu-id="bc26d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc26d-120">Here is a JSON representation of the resource.</span></span>

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