---
title: " tipo de recurso controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 89e448d828f1f7caef73b14586b06d1df238f100
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973930"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="fc93a-103">tipo de recurso controlScore</span><span class="sxs-lookup"><span data-stu-id="fc93a-103">controlScore resource type</span></span>

<span data-ttu-id="fc93a-104">Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="fc93a-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="fc93a-105">Nome</span><span class="sxs-lookup"><span data-stu-id="fc93a-105">Name</span></span> |<span data-ttu-id="fc93a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc93a-106">Type</span></span> |<span data-ttu-id="fc93a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc93a-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="fc93a-108">controlName</span><span class="sxs-lookup"><span data-stu-id="fc93a-108">controlName</span></span> |   <span data-ttu-id="fc93a-109">String</span><span class="sxs-lookup"><span data-stu-id="fc93a-109">String</span></span>  |   <span data-ttu-id="fc93a-110">Controlar o nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="fc93a-110">Control unique name</span></span> |
|   <span data-ttu-id="fc93a-111">score</span><span class="sxs-lookup"><span data-stu-id="fc93a-111">score</span></span>   |   <span data-ttu-id="fc93a-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="fc93a-112">Double</span></span>  |  <span data-ttu-id="fc93a-113">A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).</span><span class="sxs-lookup"><span data-stu-id="fc93a-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="fc93a-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="fc93a-114">controlCategory</span></span> |   <span data-ttu-id="fc93a-115">String</span><span class="sxs-lookup"><span data-stu-id="fc93a-115">String</span></span>  |  <span data-ttu-id="fc93a-116">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="fc93a-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="fc93a-117">descrição</span><span class="sxs-lookup"><span data-stu-id="fc93a-117">description</span></span> |   <span data-ttu-id="fc93a-118">String</span><span class="sxs-lookup"><span data-stu-id="fc93a-118">String</span></span>  |  <span data-ttu-id="fc93a-119">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="fc93a-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc93a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc93a-120">JSON representation</span></span>

<span data-ttu-id="fc93a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc93a-121">The following is a JSON representation of the resource.</span></span>

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
