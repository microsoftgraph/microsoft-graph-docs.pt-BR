---
title: Tipo de recurso plannerTeamsPublicationInfo
description: Contém informações detalhadas sobre o processo de publicação que criou um plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9db73bb5a914a848f3e19e079321681b22510e8e
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883227"
---
# <a name="plannerteamspublicationinfo-resource-type"></a><span data-ttu-id="b82a4-103">Tipo de recurso plannerTeamsPublicationInfo</span><span class="sxs-lookup"><span data-stu-id="b82a4-103">plannerTeamsPublicationInfo resource type</span></span>

<span data-ttu-id="b82a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b82a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b82a4-105">Contém informações detalhadas sobre o processo de publicação que criou um [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="b82a4-105">Contains detailed information about the publication process that created a [plannerTask](plannertask.md).</span></span> <span data-ttu-id="b82a4-106">Um processo de publicação cria cópias de tarefas com base em um modelo.</span><span class="sxs-lookup"><span data-stu-id="b82a4-106">A publication process creates copies of tasks based on a template.</span></span> <span data-ttu-id="b82a4-107">Essas tarefas são criadas em vários planos e têm permissões restritas para os usuários; por exemplo, eles não podem ser excluídos e os usuários podem ser impedidos de editar determinados campos.</span><span class="sxs-lookup"><span data-stu-id="b82a4-107">These tasks are created in multiple plans, and have restricted permissions for the users; for example, they cannot be deleted and users might be blocked from editing certain fields.</span></span> <span data-ttu-id="b82a4-108">A publicação é usada para distribuir tarefas em uma organização e acompanhar seu progresso centralmente.</span><span class="sxs-lookup"><span data-stu-id="b82a4-108">Publication is used to distribute tasks across an organization and track their progress centrally.</span></span>

## <a name="properties"></a><span data-ttu-id="b82a4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b82a4-109">Properties</span></span>
|<span data-ttu-id="b82a4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b82a4-110">Property</span></span>|<span data-ttu-id="b82a4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b82a4-111">Type</span></span>|<span data-ttu-id="b82a4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b82a4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b82a4-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b82a4-113">lastModifiedDateTime</span></span>|<span data-ttu-id="b82a4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b82a4-114">DateTimeOffset</span></span>|<span data-ttu-id="b82a4-115">A data e a hora em que essa tarefa foi modificada pela última vez pelo processo de publicação.</span><span class="sxs-lookup"><span data-stu-id="b82a4-115">The date and time when this task was last modified by the publication process.</span></span> <span data-ttu-id="b82a4-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b82a4-116">Read-only.</span></span> |
|<span data-ttu-id="b82a4-117">publicationId</span><span class="sxs-lookup"><span data-stu-id="b82a4-117">publicationId</span></span>|<span data-ttu-id="b82a4-118">String</span><span class="sxs-lookup"><span data-stu-id="b82a4-118">String</span></span>| <span data-ttu-id="b82a4-119">O identificador da publicação.</span><span class="sxs-lookup"><span data-stu-id="b82a4-119">The identifier of the publication.</span></span> <span data-ttu-id="b82a4-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b82a4-120">Read-only.</span></span>|
|<span data-ttu-id="b82a4-121">publishedToPlanId</span><span class="sxs-lookup"><span data-stu-id="b82a4-121">publishedToPlanId</span></span>|<span data-ttu-id="b82a4-122">String</span><span class="sxs-lookup"><span data-stu-id="b82a4-122">String</span></span>|<span data-ttu-id="b82a4-123">O identificador do **plannerPlan** em que essa tarefa foi originalmente colocada.</span><span class="sxs-lookup"><span data-stu-id="b82a4-123">The identifier of the **plannerPlan** this task was originally placed in.</span></span> <span data-ttu-id="b82a4-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b82a4-124">Read-only.</span></span> |
|<span data-ttu-id="b82a4-125">publishingTeamId</span><span class="sxs-lookup"><span data-stu-id="b82a4-125">publishingTeamId</span></span>|<span data-ttu-id="b82a4-126">String</span><span class="sxs-lookup"><span data-stu-id="b82a4-126">String</span></span>| <span data-ttu-id="b82a4-127">O identificador da equipe [que](team.md) iniciou o processo de publicação.</span><span class="sxs-lookup"><span data-stu-id="b82a4-127">The identifier of the [team](team.md) that initiated the publication process.</span></span> <span data-ttu-id="b82a4-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b82a4-128">Read-only.</span></span>|
|<span data-ttu-id="b82a4-129">publishingTeamName</span><span class="sxs-lookup"><span data-stu-id="b82a4-129">publishingTeamName</span></span>|<span data-ttu-id="b82a4-130">String</span><span class="sxs-lookup"><span data-stu-id="b82a4-130">String</span></span>|<span data-ttu-id="b82a4-131">O nome de exibição da equipe que iniciou o processo de publicação.</span><span class="sxs-lookup"><span data-stu-id="b82a4-131">The display name of the team that initiated the publication process.</span></span> <span data-ttu-id="b82a4-132">Esse nome de exibição é apenas para referência e pode não representar o nome mais atualizado da equipe.</span><span class="sxs-lookup"><span data-stu-id="b82a4-132">This display name is for reference only, and might not represent the most up-to-date name of the team.</span></span> <span data-ttu-id="b82a4-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b82a4-133">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b82a4-134">Relações</span><span class="sxs-lookup"><span data-stu-id="b82a4-134">Relationships</span></span>
<span data-ttu-id="b82a4-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b82a4-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b82a4-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b82a4-136">JSON representation</span></span>
<span data-ttu-id="b82a4-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b82a4-137">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTeamsPublicationInfo",
  "publicationId": "String",
  "publishingTeamId": "String",
  "publishingTeamName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "publishedToPlanId": "String"
}
```

