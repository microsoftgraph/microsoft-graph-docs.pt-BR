---
title: tipo de recurso controlScore
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 64b5377fce01273ab31d7ec293f5dc7a6e1342ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629282"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="3bd40-103">tipo de recurso controlScore</span><span class="sxs-lookup"><span data-stu-id="3bd40-103">controlScore resource type</span></span>

<span data-ttu-id="3bd40-104">Contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="3bd40-104">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="3bd40-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bd40-105">Properties</span></span>

|<span data-ttu-id="3bd40-106">Nome</span><span class="sxs-lookup"><span data-stu-id="3bd40-106">Name</span></span> |<span data-ttu-id="3bd40-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bd40-107">Type</span></span> |<span data-ttu-id="3bd40-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bd40-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="3bd40-109">controlName</span><span class="sxs-lookup"><span data-stu-id="3bd40-109">controlName</span></span>|<span data-ttu-id="3bd40-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bd40-110">String</span></span>|<span data-ttu-id="3bd40-111">Controlar o nome exclusivo.</span><span class="sxs-lookup"><span data-stu-id="3bd40-111">Control unique name.</span></span>|
|<span data-ttu-id="3bd40-112">score</span><span class="sxs-lookup"><span data-stu-id="3bd40-112">score</span></span>|<span data-ttu-id="3bd40-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="3bd40-113">Double</span></span>|<span data-ttu-id="3bd40-114">A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).</span><span class="sxs-lookup"><span data-stu-id="3bd40-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="3bd40-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="3bd40-115">controlCategory</span></span>|<span data-ttu-id="3bd40-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bd40-116">String</span></span>|<span data-ttu-id="3bd40-117">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="3bd40-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="3bd40-118">description</span><span class="sxs-lookup"><span data-stu-id="3bd40-118">description</span></span>|<span data-ttu-id="3bd40-119">String</span><span class="sxs-lookup"><span data-stu-id="3bd40-119">String</span></span>| <span data-ttu-id="3bd40-120">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="3bd40-120">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bd40-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bd40-121">JSON representation</span></span>

<span data-ttu-id="3bd40-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bd40-122">The following is a JSON representation of the resource.</span></span>

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
