---
title: tipo de recurso averageComparativeScore
description: Contém várias pontuações diferentes com base em escopos diferentes.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1ed82e040121f49bdef29009f6ac387ed4c79cbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532031"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="fabac-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="fabac-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="fabac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fabac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fabac-105">Contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho da indústria vertical, média por tamanho de estação da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="fabac-105">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="fabac-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fabac-106">Properties</span></span>

|<span data-ttu-id="fabac-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fabac-107">Property</span></span> |<span data-ttu-id="fabac-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fabac-108">Type</span></span> |<span data-ttu-id="fabac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fabac-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="fabac-110">base</span><span class="sxs-lookup"><span data-stu-id="fabac-110">basis</span></span>|<span data-ttu-id="fabac-111">String</span><span class="sxs-lookup"><span data-stu-id="fabac-111">String</span></span>|<span data-ttu-id="fabac-112">Tipo de escopo.</span><span class="sxs-lookup"><span data-stu-id="fabac-112">Scope type.</span></span> <span data-ttu-id="fabac-113">Os valores possíveis são: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span><span class="sxs-lookup"><span data-stu-id="fabac-113">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="fabac-114">averageScore</span><span class="sxs-lookup"><span data-stu-id="fabac-114">averageScore</span></span>|<span data-ttu-id="fabac-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="fabac-115">Double</span></span>|<span data-ttu-id="fabac-116">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="fabac-116">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fabac-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fabac-117">JSON representation</span></span>

<span data-ttu-id="fabac-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fabac-118">The following is a JSON representation of the resource.</span></span>

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
