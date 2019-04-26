---
title: " tipo de recurso controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
ms.openlocfilehash: 34e94128ff3993a01d37770bea1ad046f936405f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341180"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="ccb34-103">tipo de recurso controlScore</span><span class="sxs-lookup"><span data-stu-id="ccb34-103">controlScore resource type</span></span>

<span data-ttu-id="ccb34-104">Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="ccb34-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="ccb34-105">Nome</span><span class="sxs-lookup"><span data-stu-id="ccb34-105">Name</span></span> |<span data-ttu-id="ccb34-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccb34-106">Type</span></span> |<span data-ttu-id="ccb34-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccb34-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="ccb34-108">controlName</span><span class="sxs-lookup"><span data-stu-id="ccb34-108">controlName</span></span> |   <span data-ttu-id="ccb34-109">String</span><span class="sxs-lookup"><span data-stu-id="ccb34-109">String</span></span>  |   <span data-ttu-id="ccb34-110">Controlar o nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="ccb34-110">Control unique name</span></span> |
|   <span data-ttu-id="ccb34-111">score</span><span class="sxs-lookup"><span data-stu-id="ccb34-111">score</span></span>   |   <span data-ttu-id="ccb34-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="ccb34-112">Double</span></span>  |  <span data-ttu-id="ccb34-113">A pontuação alcançada do locatário para o controle (ele varia dia a dia, dependendo das operações do locatário no controle).</span><span class="sxs-lookup"><span data-stu-id="ccb34-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="ccb34-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="ccb34-114">controlCategory</span></span> |   <span data-ttu-id="ccb34-115">String</span><span class="sxs-lookup"><span data-stu-id="ccb34-115">String</span></span>  |  <span data-ttu-id="ccb34-116">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="ccb34-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="ccb34-117">description</span><span class="sxs-lookup"><span data-stu-id="ccb34-117">description</span></span> |   <span data-ttu-id="ccb34-118">String</span><span class="sxs-lookup"><span data-stu-id="ccb34-118">String</span></span>  |  <span data-ttu-id="ccb34-119">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="ccb34-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ccb34-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccb34-120">JSON representation</span></span>

<span data-ttu-id="ccb34-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccb34-121">The following is a JSON representation of the resource.</span></span>

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
