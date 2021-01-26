---
title: Relatórios de atividades de grupos do Microsoft 365
description: Você pode usar os relatórios de atividades de Grupos para obter informações sobre a atividade de grupos do Microsoft 365 em sua organização e ver quantos grupos do Microsoft 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7470eff43c2c77a63206cf24e0484360bf3371b6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980994"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="ae1c9-103">Relatórios de atividades de grupos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ae1c9-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="ae1c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae1c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae1c9-105">Você pode usar os relatórios de atividades de Grupos para obter informações sobre a atividade de grupos do Microsoft 365 em sua organização e ver quantos grupos do Microsoft 365 estão sendo criados e usados.</span><span class="sxs-lookup"><span data-stu-id="ae1c9-105">You can use the Groups activity reports to gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="ae1c9-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - grupos do Microsoft 365.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)</span><span class="sxs-lookup"><span data-stu-id="ae1c9-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="ae1c9-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="ae1c9-107">Reports</span></span>

| <span data-ttu-id="ae1c9-108">Função</span><span class="sxs-lookup"><span data-stu-id="ae1c9-108">Function</span></span>                                 | <span data-ttu-id="ae1c9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ae1c9-109">Return Type</span></span> | <span data-ttu-id="ae1c9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae1c9-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="ae1c9-111">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="ae1c9-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="ae1c9-112">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ae1c9-112">Stream</span></span>          | <span data-ttu-id="ae1c9-113">Obter detalhes sobre a atividade de grupos do Microsoft 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="ae1c9-113">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="ae1c9-114">Obter contagens de atividades</span><span class="sxs-lookup"><span data-stu-id="ae1c9-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="ae1c9-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ae1c9-115">Stream</span></span>          | <span data-ttu-id="ae1c9-116">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="ae1c9-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="ae1c9-117">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="ae1c9-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="ae1c9-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ae1c9-118">Stream</span></span>          | <span data-ttu-id="ae1c9-119">Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ae1c9-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="ae1c9-120">Obter armazenamento</span><span class="sxs-lookup"><span data-stu-id="ae1c9-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="ae1c9-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ae1c9-121">Stream</span></span>          | <span data-ttu-id="ae1c9-122">Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="ae1c9-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="ae1c9-123">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="ae1c9-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="ae1c9-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ae1c9-124">Stream</span></span>          | <span data-ttu-id="ae1c9-125">Obter o número total de arquivos e quantos deles estavam ativos em todos os sites de grupo associados a um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ae1c9-125">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |

