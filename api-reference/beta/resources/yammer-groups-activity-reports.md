---
title: Relatórios de atividades de grupos do Yammer
description: Você pode obter informações sobre a atividade de grupos do yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 730836b397fd11799849dcae27ae83f9db815e28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023734"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="81ab0-103">Relatórios de atividades de grupos do Yammer</span><span class="sxs-lookup"><span data-stu-id="81ab0-103">Yammer groups activity reports</span></span>

<span data-ttu-id="81ab0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81ab0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81ab0-105">Você pode obter informações sobre a atividade de grupos do yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.</span><span class="sxs-lookup"><span data-stu-id="81ab0-105">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="81ab0-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Yammer groups Activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="81ab0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="81ab0-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="81ab0-107">Reports</span></span>

| <span data-ttu-id="81ab0-108">Função</span><span class="sxs-lookup"><span data-stu-id="81ab0-108">Function</span></span>                                 | <span data-ttu-id="81ab0-109">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="81ab0-109">CSV return type</span></span> | <span data-ttu-id="81ab0-110">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="81ab0-110">JSON return type</span></span>                         | <span data-ttu-id="81ab0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="81ab0-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="81ab0-112">Obter dados de grupo</span><span class="sxs-lookup"><span data-stu-id="81ab0-112">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="81ab0-113">Fluxo</span><span class="sxs-lookup"><span data-stu-id="81ab0-113">Stream</span></span>          | [<span data-ttu-id="81ab0-114">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="81ab0-114">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="81ab0-115">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="81ab0-115">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="81ab0-116">Obter contagens de grupo</span><span class="sxs-lookup"><span data-stu-id="81ab0-116">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="81ab0-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="81ab0-117">Stream</span></span>          | [<span data-ttu-id="81ab0-118">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="81ab0-118">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="81ab0-119">Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.</span><span class="sxs-lookup"><span data-stu-id="81ab0-119">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="81ab0-120">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="81ab0-120">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="81ab0-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="81ab0-121">Stream</span></span>          | [<span data-ttu-id="81ab0-122">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="81ab0-122">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="81ab0-123">Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="81ab0-123">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |


