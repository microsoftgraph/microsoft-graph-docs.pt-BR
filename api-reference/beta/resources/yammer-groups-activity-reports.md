---
title: Relatórios de atividades de grupos do Yammer
description: Você pode obter ideias para a atividade do Yammer grupos em sua organização e ver quantos grupos do Yammer estão sendo criadas e usadas.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 05e5826a85e7d2e37af82cdf6277857746b1b922
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514156"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="631c2-103">Relatórios de atividades de grupos do Yammer</span><span class="sxs-lookup"><span data-stu-id="631c2-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="631c2-104">Você pode obter ideias para a atividade do Yammer grupos em sua organização e ver quantos grupos do Yammer estão sendo criadas e usadas.</span><span class="sxs-lookup"><span data-stu-id="631c2-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="631c2-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="631c2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="631c2-106">Relatórios</span><span class="sxs-lookup"><span data-stu-id="631c2-106">Reports</span></span>

| <span data-ttu-id="631c2-107">Função</span><span class="sxs-lookup"><span data-stu-id="631c2-107">Function</span></span>                                 | <span data-ttu-id="631c2-108">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="631c2-108">CSV return type</span></span> | <span data-ttu-id="631c2-109">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="631c2-109">JSON return type</span></span>                         | <span data-ttu-id="631c2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="631c2-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="631c2-111">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="631c2-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="631c2-112">Stream</span><span class="sxs-lookup"><span data-stu-id="631c2-112">Stream</span></span>          | [<span data-ttu-id="631c2-113">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="631c2-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="631c2-114">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="631c2-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="631c2-115">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="631c2-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="631c2-116">Stream</span><span class="sxs-lookup"><span data-stu-id="631c2-116">Stream</span></span>          | [<span data-ttu-id="631c2-117">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="631c2-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="631c2-118">Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.</span><span class="sxs-lookup"><span data-stu-id="631c2-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="631c2-119">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="631c2-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="631c2-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="631c2-120">Stream</span></span>          | [<span data-ttu-id="631c2-121">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="631c2-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="631c2-122">Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="631c2-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
