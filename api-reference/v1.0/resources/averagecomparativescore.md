---
title: tipo de recurso averageComparativeScore
description: Contém várias pontuações diferentes com base em escopos diferentes.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 59faa1c3dcf3f7f2b70807a74878dab796ae4d54
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629324"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="4b7a2-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="4b7a2-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="4b7a2-104">Contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho da indústria vertical, média por tamanho de estação da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="4b7a2-104">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="4b7a2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b7a2-105">Properties</span></span>

|<span data-ttu-id="4b7a2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b7a2-106">Property</span></span> |<span data-ttu-id="4b7a2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b7a2-107">Type</span></span> |<span data-ttu-id="4b7a2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b7a2-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="4b7a2-109">base</span><span class="sxs-lookup"><span data-stu-id="4b7a2-109">basis</span></span>|<span data-ttu-id="4b7a2-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b7a2-110">String</span></span>|<span data-ttu-id="4b7a2-111">Tipo de escopo.</span><span class="sxs-lookup"><span data-stu-id="4b7a2-111">Scope type.</span></span> <span data-ttu-id="4b7a2-112">Os valores possíveis são: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span><span class="sxs-lookup"><span data-stu-id="4b7a2-112">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="4b7a2-113">averageScore</span><span class="sxs-lookup"><span data-stu-id="4b7a2-113">averageScore</span></span>|<span data-ttu-id="4b7a2-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="4b7a2-114">Double</span></span>|<span data-ttu-id="4b7a2-115">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="4b7a2-115">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b7a2-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b7a2-116">JSON representation</span></span>

<span data-ttu-id="4b7a2-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b7a2-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
