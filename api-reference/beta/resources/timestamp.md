---
title: tipo de recurso da carimbo de hora
description: Data e hora informações para um ponto no tempo.
ms.openlocfilehash: 24326f0c104dd4ee2be80016ce798cc843288975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036679"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="ded44-103">tipo de recurso da carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="ded44-103">timeStamp resource type</span></span>

> <span data-ttu-id="ded44-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ded44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ded44-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ded44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ded44-106">Data e hora informações para um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="ded44-106">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ded44-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ded44-107">JSON representation</span></span>

<span data-ttu-id="ded44-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ded44-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="ded44-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ded44-109">Properties</span></span>
| <span data-ttu-id="ded44-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ded44-110">Property</span></span>     | <span data-ttu-id="ded44-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ded44-111">Type</span></span>   |<span data-ttu-id="ded44-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ded44-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ded44-113">data</span><span class="sxs-lookup"><span data-stu-id="ded44-113">date</span></span>|<span data-ttu-id="ded44-114">Data</span><span class="sxs-lookup"><span data-stu-id="ded44-114">Date</span></span>|<span data-ttu-id="ded44-115">A parte da data do carimbo de hora.</span><span class="sxs-lookup"><span data-stu-id="ded44-115">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="ded44-116">time</span><span class="sxs-lookup"><span data-stu-id="ded44-116">time</span></span>|<span data-ttu-id="ded44-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ded44-117">TimeOfDay</span></span>|<span data-ttu-id="ded44-118">A parte do tempo do carimbo de hora.</span><span class="sxs-lookup"><span data-stu-id="ded44-118">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="ded44-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="ded44-119">timeZone</span></span>|<span data-ttu-id="ded44-120">String</span><span class="sxs-lookup"><span data-stu-id="ded44-120">String</span></span>|<span data-ttu-id="ded44-121">A porção de fuso horário da carimbo de hora, o que é uma das áreas longitudinal 24 no mundo.</span><span class="sxs-lookup"><span data-stu-id="ded44-121">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->