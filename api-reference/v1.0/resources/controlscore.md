---
title: tipo de recurso controlScore
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e4470d1ce22f5ffbf3c805adc5328398d57d9fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056921"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="4707d-103">tipo de recurso controlScore</span><span class="sxs-lookup"><span data-stu-id="4707d-103">controlScore resource type</span></span>

<span data-ttu-id="4707d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4707d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4707d-105">Contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="4707d-105">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="4707d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4707d-106">Properties</span></span>

|<span data-ttu-id="4707d-107">Nome</span><span class="sxs-lookup"><span data-stu-id="4707d-107">Name</span></span> |<span data-ttu-id="4707d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4707d-108">Type</span></span> |<span data-ttu-id="4707d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4707d-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="4707d-110">controlName</span><span class="sxs-lookup"><span data-stu-id="4707d-110">controlName</span></span>|<span data-ttu-id="4707d-111">String</span><span class="sxs-lookup"><span data-stu-id="4707d-111">String</span></span>|<span data-ttu-id="4707d-112">Controlar o nome exclusivo.</span><span class="sxs-lookup"><span data-stu-id="4707d-112">Control unique name.</span></span>|
|<span data-ttu-id="4707d-113">Pontuação</span><span class="sxs-lookup"><span data-stu-id="4707d-113">score</span></span>|<span data-ttu-id="4707d-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="4707d-114">Double</span></span>|<span data-ttu-id="4707d-115">A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).</span><span class="sxs-lookup"><span data-stu-id="4707d-115">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="4707d-116">controlCategory</span><span class="sxs-lookup"><span data-stu-id="4707d-116">controlCategory</span></span>|<span data-ttu-id="4707d-117">String</span><span class="sxs-lookup"><span data-stu-id="4707d-117">String</span></span>|<span data-ttu-id="4707d-118">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="4707d-118">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="4707d-119">description</span><span class="sxs-lookup"><span data-stu-id="4707d-119">description</span></span>|<span data-ttu-id="4707d-120">String</span><span class="sxs-lookup"><span data-stu-id="4707d-120">String</span></span>| <span data-ttu-id="4707d-121">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="4707d-121">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4707d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4707d-122">JSON representation</span></span>

<span data-ttu-id="4707d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4707d-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

