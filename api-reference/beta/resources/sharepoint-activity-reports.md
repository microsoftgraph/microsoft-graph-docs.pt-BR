---
title: Relatório de atividades do SharePoint
description: Você pode obter a atividade de cada usuário licenciado para usar o SharePoint analisando sua interação com os arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 2e7b834f9bd4e1a440f0fd5167679ce0074668cd
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983780"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="fd921-104">Relatório de atividades do SharePoint</span><span class="sxs-lookup"><span data-stu-id="fd921-104">SharePoint activity reports</span></span>

<span data-ttu-id="fd921-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd921-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd921-106">Você pode obter a atividade de cada usuário licenciado para usar o SharePoint analisando sua interação com os arquivos.</span><span class="sxs-lookup"><span data-stu-id="fd921-106">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="fd921-107">Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="fd921-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="fd921-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - Atividade do SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="fd921-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="fd921-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="fd921-109">Reports</span></span>

| <span data-ttu-id="fd921-110">Função</span><span class="sxs-lookup"><span data-stu-id="fd921-110">Function</span></span>                                 | <span data-ttu-id="fd921-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="fd921-111">CSV Return Type</span></span> | <span data-ttu-id="fd921-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="fd921-112">JSON Return Type</span></span>                         | <span data-ttu-id="fd921-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd921-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="fd921-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="fd921-114">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="fd921-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="fd921-115">Stream</span></span>          | [<span data-ttu-id="fd921-116">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fd921-116">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="fd921-117">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="fd921-117">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="fd921-118">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="fd921-118">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="fd921-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="fd921-119">Stream</span></span>          | [<span data-ttu-id="fd921-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="fd921-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="fd921-121">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fd921-121">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="fd921-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="fd921-122">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="fd921-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="fd921-123">Stream</span></span>          | [<span data-ttu-id="fd921-124">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="fd921-124">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="fd921-125">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="fd921-125">Get the trend in the number of active users.</span></span> <span data-ttu-id="fd921-126">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="fd921-126">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="fd921-127">Obter páginas</span><span class="sxs-lookup"><span data-stu-id="fd921-127">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="fd921-128">Fluxo</span><span class="sxs-lookup"><span data-stu-id="fd921-128">Stream</span></span>          | [<span data-ttu-id="fd921-129">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="fd921-129">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="fd921-130">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="fd921-130">Get the number of unique pages visited by users.</span></span> |


