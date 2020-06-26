---
title: Relatórios de atividades de grupos do Yammer
description: Você pode obter informações sobre a atividade de grupos do yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: cdeb94c9b5b687ab9584a236daaafb7c018a809c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897467"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="6e573-103">Relatórios de atividades de grupos do Yammer</span><span class="sxs-lookup"><span data-stu-id="6e573-103">Yammer groups activity reports</span></span>

<span data-ttu-id="6e573-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e573-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e573-105">Você pode obter informações sobre a atividade de grupos do yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.</span><span class="sxs-lookup"><span data-stu-id="6e573-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="6e573-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Yammer groups Activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="6e573-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="6e573-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="6e573-107">Reports</span></span>

| <span data-ttu-id="6e573-108">Função</span><span class="sxs-lookup"><span data-stu-id="6e573-108">Function</span></span>                                 | <span data-ttu-id="6e573-109">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="6e573-109">CSV return type</span></span> | <span data-ttu-id="6e573-110">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="6e573-110">JSON return type</span></span>                         | <span data-ttu-id="6e573-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e573-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="6e573-112">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="6e573-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="6e573-113">Stream</span><span class="sxs-lookup"><span data-stu-id="6e573-113">Stream</span></span>          | [<span data-ttu-id="6e573-114">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="6e573-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="6e573-115">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="6e573-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="6e573-116">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="6e573-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="6e573-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="6e573-117">Stream</span></span>          | [<span data-ttu-id="6e573-118">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="6e573-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="6e573-119">Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.</span><span class="sxs-lookup"><span data-stu-id="6e573-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="6e573-120">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="6e573-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="6e573-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="6e573-121">Stream</span></span>          | [<span data-ttu-id="6e573-122">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6e573-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="6e573-123">Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="6e573-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
