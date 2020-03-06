---
title: Relatórios de atividades dos Grupos do Office 365
description: Você pode usar os relatórios de atividades dos Grupos para obter informações sobre a atividade dos Grupos do Office 365 em sua organização e ver quantos Grupos do Office 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 57749ca15e4eaf4aad14f3f914426d861ea45eeb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534180"
---
# <a name="office-365-groups-activity-reports"></a><span data-ttu-id="23acf-103">Relatórios de atividades dos Grupos do Office 365</span><span class="sxs-lookup"><span data-stu-id="23acf-103">Office 365 Groups activity reports</span></span>

<span data-ttu-id="23acf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23acf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23acf-105">Você pode usar os relatórios de atividades dos Grupos para obter informações sobre a atividade dos Grupos do Office 365 em sua organização e ver quantos Grupos do Office 365 estão sendo criados e usados.</span><span class="sxs-lookup"><span data-stu-id="23acf-105">You can use the Groups activity reports to gain insights into the activity of Office 365 Groups in your organization and see how many Office 365 Groups are being created and used.</span></span>

> <span data-ttu-id="23acf-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="23acf-106">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="reports"></a><span data-ttu-id="23acf-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="23acf-107">Reports</span></span>

| <span data-ttu-id="23acf-108">Função</span><span class="sxs-lookup"><span data-stu-id="23acf-108">Function</span></span>                                 | <span data-ttu-id="23acf-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23acf-109">Return Type</span></span> | <span data-ttu-id="23acf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23acf-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [<span data-ttu-id="23acf-111">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="23acf-111">Get group detail</span></span>](../api/reportroot-getoffice365groupsactivitydetail.md) | <span data-ttu-id="23acf-112">Stream</span><span class="sxs-lookup"><span data-stu-id="23acf-112">Stream</span></span>          | <span data-ttu-id="23acf-113">Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.</span><span class="sxs-lookup"><span data-stu-id="23acf-113">Get details about Office 365 Groups activity by group.</span></span> |
| [<span data-ttu-id="23acf-114">Obter contagens de atividades</span><span class="sxs-lookup"><span data-stu-id="23acf-114">Get activity counts</span></span>](../api/reportroot-getoffice365groupsactivitycounts.md) | <span data-ttu-id="23acf-115">Stream</span><span class="sxs-lookup"><span data-stu-id="23acf-115">Stream</span></span>          | <span data-ttu-id="23acf-116">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="23acf-116">Get the number of group activities across group workloads.</span></span> |
| [<span data-ttu-id="23acf-117">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="23acf-117">Get group counts</span></span>](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | <span data-ttu-id="23acf-118">Stream</span><span class="sxs-lookup"><span data-stu-id="23acf-118">Stream</span></span>          | <span data-ttu-id="23acf-119">Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="23acf-119">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span> |
| [<span data-ttu-id="23acf-120">Obter armazenamento</span><span class="sxs-lookup"><span data-stu-id="23acf-120">Get storage</span></span>](../api/reportroot-getoffice365groupsactivitystorage.md) | <span data-ttu-id="23acf-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="23acf-121">Stream</span></span>          | <span data-ttu-id="23acf-122">Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="23acf-122">Get the total storage used across all group mailboxes and group sites.</span></span> |
| [<span data-ttu-id="23acf-123">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="23acf-123">Get file counts</span></span>](../api/reportroot-getoffice365groupsactivityfilecounts.md) | <span data-ttu-id="23acf-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="23acf-124">Stream</span></span>          | <span data-ttu-id="23acf-125">Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="23acf-125">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span> |
