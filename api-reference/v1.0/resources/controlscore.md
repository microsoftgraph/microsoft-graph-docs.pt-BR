---
title: tipo de recurso controlScore
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 68e4bf278b7d1b6ea6f00f75192847abab1ae3a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032841"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="00083-103">tipo de recurso controlScore</span><span class="sxs-lookup"><span data-stu-id="00083-103">controlScore resource type</span></span>

<span data-ttu-id="00083-104">Contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="00083-104">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="00083-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00083-105">Properties</span></span>

|<span data-ttu-id="00083-106">Nome</span><span class="sxs-lookup"><span data-stu-id="00083-106">Name</span></span> |<span data-ttu-id="00083-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="00083-107">Type</span></span> |<span data-ttu-id="00083-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="00083-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="00083-109">controlName</span><span class="sxs-lookup"><span data-stu-id="00083-109">controlName</span></span>|<span data-ttu-id="00083-110">String</span><span class="sxs-lookup"><span data-stu-id="00083-110">String</span></span>|<span data-ttu-id="00083-111">Controlar o nome exclusivo.</span><span class="sxs-lookup"><span data-stu-id="00083-111">Control unique name.</span></span>|
|<span data-ttu-id="00083-112">score</span><span class="sxs-lookup"><span data-stu-id="00083-112">score</span></span>|<span data-ttu-id="00083-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="00083-113">Double</span></span>|<span data-ttu-id="00083-114">A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).</span><span class="sxs-lookup"><span data-stu-id="00083-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="00083-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="00083-115">controlCategory</span></span>|<span data-ttu-id="00083-116">String</span><span class="sxs-lookup"><span data-stu-id="00083-116">String</span></span>|<span data-ttu-id="00083-117">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="00083-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="00083-118">descrição</span><span class="sxs-lookup"><span data-stu-id="00083-118">description</span></span>|<span data-ttu-id="00083-119">String</span><span class="sxs-lookup"><span data-stu-id="00083-119">String</span></span>| <span data-ttu-id="00083-120">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="00083-120">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00083-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00083-121">JSON representation</span></span>

<span data-ttu-id="00083-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00083-122">The following is a JSON representation of the resource.</span></span>

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
