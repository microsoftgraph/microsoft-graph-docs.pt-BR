---
title: Relatórios de atividades do Microsoft 365 groups
description: Você pode usar os relatórios de atividades de grupos para obter informações sobre a atividade dos grupos do Microsoft 365 em sua organização e ver quantos grupos da Microsoft 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 52bb3cb71837f049cada3970bdd0faa710f38844
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965418"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="e8177-103">Relatórios de atividades do Microsoft 365 groups</span><span class="sxs-lookup"><span data-stu-id="e8177-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="e8177-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8177-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8177-105">Você pode usar os relatórios de atividades de grupos para obter informações sobre a atividade dos grupos do Microsoft 365 em sua organização e ver quantos grupos da Microsoft 365 estão sendo criados e usados.</span><span class="sxs-lookup"><span data-stu-id="e8177-105">You can use the Groups activity reports to gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="e8177-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="e8177-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="e8177-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="e8177-107">Reports</span></span>

| <span data-ttu-id="e8177-108">Função</span><span class="sxs-lookup"><span data-stu-id="e8177-108">Function</span></span>                                 | <span data-ttu-id="e8177-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e8177-109">Return Type</span></span> | <span data-ttu-id="e8177-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8177-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="e8177-111">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="e8177-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="e8177-112">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e8177-112">Stream</span></span>          | <span data-ttu-id="e8177-113">Obtenha detalhes sobre a atividade de grupos do Microsoft 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="e8177-113">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="e8177-114">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="e8177-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="e8177-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e8177-115">Stream</span></span>          | <span data-ttu-id="e8177-116">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="e8177-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="e8177-117">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="e8177-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="e8177-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e8177-118">Stream</span></span>          | <span data-ttu-id="e8177-119">Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e8177-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="e8177-120">Obter armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8177-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="e8177-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e8177-121">Stream</span></span>          | <span data-ttu-id="e8177-122">Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="e8177-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="e8177-123">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="e8177-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="e8177-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e8177-124">Stream</span></span>          | <span data-ttu-id="e8177-125">Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites de grupo associados a um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e8177-125">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |

