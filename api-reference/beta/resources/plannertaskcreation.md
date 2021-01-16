---
title: Tipo de recurso plannerTaskCreation
description: Contém informações sobre a origem do plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e8a2a4bf3aae5f23a04c7ecb8ad043631f946b20
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883228"
---
# <a name="plannertaskcreation-resource-type"></a><span data-ttu-id="802df-103">Tipo de recurso plannerTaskCreation</span><span class="sxs-lookup"><span data-stu-id="802df-103">plannerTaskCreation resource type</span></span>

<span data-ttu-id="802df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="802df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="802df-105">Contém informações sobre a origem do [plannerTask](plannerTask.md).</span><span class="sxs-lookup"><span data-stu-id="802df-105">Contains information about the origin of the [plannerTask](plannerTask.md).</span></span> <span data-ttu-id="802df-106">Esse recurso terá todas as suas propriedades definidas como ou exatamente uma propriedade terá um valor que indica que a tarefa foi criada pelo processo descrito `null` por essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="802df-106">This resource will either have all its properties set to `null`, or exactly one property will have a value that indicates that the task was created by the process described by that property.</span></span> <span data-ttu-id="802df-107">Todas as `null` propriedades indicam que essa tarefa não foi criada por nenhum processo especializado.</span><span class="sxs-lookup"><span data-stu-id="802df-107">All properties `null` indicates this task was not created by any specialized process.</span></span> <span data-ttu-id="802df-108">Os aplicativos não precisam saber a origem da tarefa para poder trabalhar com ela; No entanto, alguns aplicativos podem usar as informações adicionais para fornecer experiências específicas em torno dessas tarefas.</span><span class="sxs-lookup"><span data-stu-id="802df-108">Apps do not need to know the origin of the task to be able to work with it; however, some apps can use the additional information to provide specific experiences around these tasks.</span></span> <span data-ttu-id="802df-109">Consulte a documentação para recursos específicos para saber mais.</span><span class="sxs-lookup"><span data-stu-id="802df-109">See the documentation for specific resources to learn more.</span></span>

## <a name="properties"></a><span data-ttu-id="802df-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="802df-110">Properties</span></span>
|<span data-ttu-id="802df-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="802df-111">Property</span></span>|<span data-ttu-id="802df-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="802df-112">Type</span></span>|<span data-ttu-id="802df-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="802df-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="802df-114">teamsPublicationInfo</span><span class="sxs-lookup"><span data-stu-id="802df-114">teamsPublicationInfo</span></span>|[<span data-ttu-id="802df-115">plannerTeamsPublicationInfo</span><span class="sxs-lookup"><span data-stu-id="802df-115">plannerTeamsPublicationInfo</span></span>](../resources/plannerteamspublicationinfo.md)|<span data-ttu-id="802df-116">Informações sobre o processo de publicação que criou essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="802df-116">Information about the publication process that created this task.</span></span> <span data-ttu-id="802df-117">`null` indica que a tarefa não foi criada por um processo de publicação.</span><span class="sxs-lookup"><span data-stu-id="802df-117">`null` value indicates that the task was not created by a publication process.</span></span>|

## <a name="relationships"></a><span data-ttu-id="802df-118">Relações</span><span class="sxs-lookup"><span data-stu-id="802df-118">Relationships</span></span>
<span data-ttu-id="802df-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="802df-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="802df-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="802df-120">JSON representation</span></span>
<span data-ttu-id="802df-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="802df-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTaskCreation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTaskCreation",
  "teamsPublicationInfo": {
    "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
  }
}
```

