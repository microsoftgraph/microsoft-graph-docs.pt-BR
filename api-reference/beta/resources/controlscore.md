---
title: " tipo de recurso controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2b718851d1a27c3317a0ce77554be7ea3f8906a4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811494"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="cc8ef-103">tipo de recurso controlScore</span><span class="sxs-lookup"><span data-stu-id="cc8ef-103">controlScore resource type</span></span>

<span data-ttu-id="cc8ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc8ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc8ef-105">Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="cc8ef-105">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="cc8ef-106">Nome</span><span class="sxs-lookup"><span data-stu-id="cc8ef-106">Name</span></span> |<span data-ttu-id="cc8ef-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc8ef-107">Type</span></span> |<span data-ttu-id="cc8ef-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc8ef-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="cc8ef-109">controlName</span><span class="sxs-lookup"><span data-stu-id="cc8ef-109">controlName</span></span> |   <span data-ttu-id="cc8ef-110">String</span><span class="sxs-lookup"><span data-stu-id="cc8ef-110">String</span></span>  |   <span data-ttu-id="cc8ef-111">Controlar o nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="cc8ef-111">Control unique name</span></span> |
|   <span data-ttu-id="cc8ef-112">Pontuação</span><span class="sxs-lookup"><span data-stu-id="cc8ef-112">score</span></span>   |   <span data-ttu-id="cc8ef-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="cc8ef-113">Double</span></span>  |  <span data-ttu-id="cc8ef-114">A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).</span><span class="sxs-lookup"><span data-stu-id="cc8ef-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="cc8ef-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="cc8ef-115">controlCategory</span></span> |   <span data-ttu-id="cc8ef-116">String</span><span class="sxs-lookup"><span data-stu-id="cc8ef-116">String</span></span>  |  <span data-ttu-id="cc8ef-117">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="cc8ef-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="cc8ef-118">description</span><span class="sxs-lookup"><span data-stu-id="cc8ef-118">description</span></span> |   <span data-ttu-id="cc8ef-119">String</span><span class="sxs-lookup"><span data-stu-id="cc8ef-119">String</span></span>  |  <span data-ttu-id="cc8ef-120">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="cc8ef-120">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc8ef-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc8ef-121">JSON representation</span></span>

<span data-ttu-id="cc8ef-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc8ef-122">The following is a JSON representation of the resource.</span></span>

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
