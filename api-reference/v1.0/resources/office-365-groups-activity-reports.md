---
title: Relatórios de atividades do Microsoft 365 groups
description: Você pode usar os relatórios de atividades de grupos para obter informações sobre a atividade dos grupos do Microsoft 365 em sua organização e ver quantos grupos da Microsoft 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0cd0dfc07813714d376a38125835917c712e7ebe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898153"
---
# <a name="microsoft-365-groups-activity-reports"></a><span data-ttu-id="012ba-103">Relatórios de atividades do Microsoft 365 groups</span><span class="sxs-lookup"><span data-stu-id="012ba-103">Microsoft 365 groups activity reports</span></span>

<span data-ttu-id="012ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="012ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="012ba-105">Você pode usar os relatórios de atividades de grupos para obter informações sobre a atividade dos grupos do Microsoft 365 em sua organização e ver quantos grupos da Microsoft 365 estão sendo criados e usados.</span><span class="sxs-lookup"><span data-stu-id="012ba-105">You can use the Groups activity reports to gain insights into the activity of Microsoft 365 groups in your organization and see how many Microsoft 365 groups are being created and used.</span></span>

> <span data-ttu-id="012ba-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="012ba-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="012ba-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="012ba-107">Reports</span></span>

| <span data-ttu-id="012ba-108">Função</span><span class="sxs-lookup"><span data-stu-id="012ba-108">Function</span></span>                                 | <span data-ttu-id="012ba-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="012ba-109">Return Type</span></span> | <span data-ttu-id="012ba-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="012ba-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="012ba-111">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="012ba-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="012ba-112">Stream</span><span class="sxs-lookup"><span data-stu-id="012ba-112">Stream</span></span>          | <span data-ttu-id="012ba-113">Obtenha detalhes sobre a atividade de grupos do Microsoft 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="012ba-113">Get details about Microsoft 365 groups activity by group.</span></span> |
| [<span data-ttu-id="012ba-114">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="012ba-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="012ba-115">Stream</span><span class="sxs-lookup"><span data-stu-id="012ba-115">Stream</span></span>          | <span data-ttu-id="012ba-116">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="012ba-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="012ba-117">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="012ba-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="012ba-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="012ba-118">Stream</span></span>          | <span data-ttu-id="012ba-119">Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="012ba-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="012ba-120">Obter armazenamento</span><span class="sxs-lookup"><span data-stu-id="012ba-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="012ba-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="012ba-121">Stream</span></span>          | <span data-ttu-id="012ba-122">Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="012ba-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="012ba-123">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="012ba-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="012ba-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="012ba-124">Stream</span></span>          | <span data-ttu-id="012ba-125">Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites de grupo associados a um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="012ba-125">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span> |
