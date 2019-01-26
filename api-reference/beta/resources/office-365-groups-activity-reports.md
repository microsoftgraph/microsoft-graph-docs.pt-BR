---
title: Relatórios de atividades dos Grupos do Office 365
description: Você pode obter ideias para a atividade do Office 365 grupos em sua organização e ver quantos grupos do Office 365 estão sendo criadas e usadas.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e698a1096d244b864bbb15cf06c16e8cf79ff1f2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572196"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="bab44-103">Relatórios de atividades dos Grupos do Office 365</span><span class="sxs-lookup"><span data-stu-id="bab44-103">Office 365 Groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bab44-104">Você pode obter ideias para a atividade do Office 365 grupos em sua organização e ver quantos grupos do Office 365 estão sendo criadas e usadas.</span><span class="sxs-lookup"><span data-stu-id="bab44-104">You can gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 groups are being created and used.</span></span>

> <span data-ttu-id="bab44-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="bab44-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="bab44-106">Relatórios</span><span class="sxs-lookup"><span data-stu-id="bab44-106">Reports</span></span>

| <span data-ttu-id="bab44-107">Função</span><span class="sxs-lookup"><span data-stu-id="bab44-107">Function</span></span>                                 | <span data-ttu-id="bab44-108">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="bab44-108">CSV return type</span></span> | <span data-ttu-id="bab44-109">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="bab44-109">JSON return type</span></span>                         | <span data-ttu-id="bab44-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bab44-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="bab44-111">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="bab44-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="bab44-112">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bab44-112">Stream</span></span>          | [<span data-ttu-id="bab44-113">office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="bab44-113">office365GroupsActivityDetail</span></span>](../resources/office365groupsactivitydetail.md) | <span data-ttu-id="bab44-114">Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="bab44-114">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="bab44-115">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="bab44-115">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="bab44-116">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bab44-116">Stream</span></span>          | [<span data-ttu-id="bab44-117">office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="bab44-117">office365GroupsActivityCounts</span></span>](../resources/office365groupsactivitycounts.md) | <span data-ttu-id="bab44-118">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="bab44-118">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="bab44-119">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="bab44-119">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="bab44-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bab44-120">Stream</span></span>          | [<span data-ttu-id="bab44-121">office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="bab44-121">office365GroupsActivityGroupCounts</span></span>](../resources/office365groupsactivitygroupcounts.md) | <span data-ttu-id="bab44-122">Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bab44-122">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="bab44-123">Obter armazenamento</span><span class="sxs-lookup"><span data-stu-id="bab44-123">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="bab44-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bab44-124">Stream</span></span>          | [<span data-ttu-id="bab44-125">office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="bab44-125">office365GroupsActivityStorage</span></span>](../resources/office365groupsactivitystorage.md) | <span data-ttu-id="bab44-126">Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="bab44-126">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="bab44-127">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="bab44-127">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="bab44-128">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bab44-128">Stream</span></span>          | [<span data-ttu-id="bab44-129">office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="bab44-129">office365GroupsActivityFileCounts</span></span>](../resources/office365groupsactivityfilecounts.md) | <span data-ttu-id="bab44-130">Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="bab44-130">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
