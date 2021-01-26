---
title: Relatórios de atividades de grupos do Yammer
description: Você pode obter informações sobre a atividade de grupos do Yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 09c8aa8476886f8bbf7266817449195b4c07aa05
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982422"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="d8d56-103">Relatórios de atividades de grupos do Yammer</span><span class="sxs-lookup"><span data-stu-id="d8d56-103">Yammer groups activity reports</span></span>

<span data-ttu-id="d8d56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8d56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8d56-105">Você pode obter informações sobre a atividade de grupos do Yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.</span><span class="sxs-lookup"><span data-stu-id="d8d56-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="d8d56-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira [relatórios do Microsoft 365 - atividade de grupos do Yammer.](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)</span><span class="sxs-lookup"><span data-stu-id="d8d56-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="d8d56-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="d8d56-107">Reports</span></span>

| <span data-ttu-id="d8d56-108">Função</span><span class="sxs-lookup"><span data-stu-id="d8d56-108">Function</span></span>                                 | <span data-ttu-id="d8d56-109">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="d8d56-109">CSV return type</span></span> | <span data-ttu-id="d8d56-110">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="d8d56-110">JSON return type</span></span>                         | <span data-ttu-id="d8d56-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d56-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d8d56-112">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="d8d56-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="d8d56-113">Fluxo</span><span class="sxs-lookup"><span data-stu-id="d8d56-113">Stream</span></span>          | [<span data-ttu-id="d8d56-114">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="d8d56-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="d8d56-115">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="d8d56-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="d8d56-116">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="d8d56-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="d8d56-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="d8d56-117">Stream</span></span>          | [<span data-ttu-id="d8d56-118">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="d8d56-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="d8d56-119">Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.</span><span class="sxs-lookup"><span data-stu-id="d8d56-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="d8d56-120">Obter contagens de atividades</span><span class="sxs-lookup"><span data-stu-id="d8d56-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="d8d56-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="d8d56-121">Stream</span></span>          | [<span data-ttu-id="d8d56-122">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d8d56-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="d8d56-123">Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="d8d56-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |


