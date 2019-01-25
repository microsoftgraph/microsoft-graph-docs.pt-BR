---
title: tipo de recurso usageDetails
description: Tipo complexo que contém as propriedades de itens usados. Obter informações sobre quando o recurso foi acessado pela última vez (exibidos) e modificado (editado) pelo usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4df15bf635785aba054d52beb89b5ac04d48d3d3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526827"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="53dee-104">tipo de recurso usageDetails</span><span class="sxs-lookup"><span data-stu-id="53dee-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53dee-105">Tipo complexo que contém as propriedades de itens [usado](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="53dee-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="53dee-106">Obter informações sobre quando o recurso foi acessado pela última vez (exibidos) e modificado (editado) pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="53dee-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53dee-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53dee-107">JSON representation</span></span>

<span data-ttu-id="53dee-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="53dee-108">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="53dee-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53dee-109">Properties</span></span>

| <span data-ttu-id="53dee-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53dee-110">Property</span></span>              | <span data-ttu-id="53dee-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="53dee-111">Type</span></span>          | <span data-ttu-id="53dee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="53dee-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="53dee-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="53dee-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="53dee-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53dee-114">DateTimeOffset</span></span>        | <span data-ttu-id="53dee-115">A data e hora que o recurso foi acessado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="53dee-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="53dee-116">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="53dee-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53dee-117">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="53dee-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="53dee-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53dee-118">Read-only.</span></span>                      |
| <span data-ttu-id="53dee-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53dee-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="53dee-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53dee-120">DateTimeOffset</span></span>        | <span data-ttu-id="53dee-121">A data e hora que o recurso da última modificação pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="53dee-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="53dee-122">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="53dee-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53dee-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="53dee-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="53dee-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53dee-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
