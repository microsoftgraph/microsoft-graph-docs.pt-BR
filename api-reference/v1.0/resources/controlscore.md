---
title: tipo de recurso controlScore
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc3de6363784f62792d7c4e56906c79ed1be0c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531768"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="27c69-103">tipo de recurso controlScore</span><span class="sxs-lookup"><span data-stu-id="27c69-103">controlScore resource type</span></span>

<span data-ttu-id="27c69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27c69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27c69-105">Contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="27c69-105">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="27c69-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27c69-106">Properties</span></span>

|<span data-ttu-id="27c69-107">Nome</span><span class="sxs-lookup"><span data-stu-id="27c69-107">Name</span></span> |<span data-ttu-id="27c69-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="27c69-108">Type</span></span> |<span data-ttu-id="27c69-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="27c69-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="27c69-110">controlName</span><span class="sxs-lookup"><span data-stu-id="27c69-110">controlName</span></span>|<span data-ttu-id="27c69-111">String</span><span class="sxs-lookup"><span data-stu-id="27c69-111">String</span></span>|<span data-ttu-id="27c69-112">Controlar o nome exclusivo.</span><span class="sxs-lookup"><span data-stu-id="27c69-112">Control unique name.</span></span>|
|<span data-ttu-id="27c69-113">score</span><span class="sxs-lookup"><span data-stu-id="27c69-113">score</span></span>|<span data-ttu-id="27c69-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="27c69-114">Double</span></span>|<span data-ttu-id="27c69-115">A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).</span><span class="sxs-lookup"><span data-stu-id="27c69-115">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="27c69-116">controlCategory</span><span class="sxs-lookup"><span data-stu-id="27c69-116">controlCategory</span></span>|<span data-ttu-id="27c69-117">String</span><span class="sxs-lookup"><span data-stu-id="27c69-117">String</span></span>|<span data-ttu-id="27c69-118">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="27c69-118">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="27c69-119">description</span><span class="sxs-lookup"><span data-stu-id="27c69-119">description</span></span>|<span data-ttu-id="27c69-120">String</span><span class="sxs-lookup"><span data-stu-id="27c69-120">String</span></span>| <span data-ttu-id="27c69-121">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="27c69-121">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27c69-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27c69-122">JSON representation</span></span>

<span data-ttu-id="27c69-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27c69-123">The following is a JSON representation of the resource.</span></span>

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
