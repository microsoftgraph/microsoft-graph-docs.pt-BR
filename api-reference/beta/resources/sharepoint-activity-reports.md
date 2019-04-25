---
title: Relatório de atividades do SharePoint
description: Você pode obter a atividade de cada usuário licenciado para usar o SharePoint examinando sua interação com os arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 98d0393545963a73852197f5bd78241cfb958a22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584087"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="202fe-104">Relatório de atividades do SharePoint</span><span class="sxs-lookup"><span data-stu-id="202fe-104">SharePoint activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="202fe-105">Você pode obter a atividade de cada usuário licenciado para usar o SharePoint examinando sua interação com os arquivos.</span><span class="sxs-lookup"><span data-stu-id="202fe-105">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="202fe-106">Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="202fe-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="202fe-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="202fe-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="202fe-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="202fe-108">Reports</span></span>

| <span data-ttu-id="202fe-109">Função</span><span class="sxs-lookup"><span data-stu-id="202fe-109">Function</span></span>                                 | <span data-ttu-id="202fe-110">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="202fe-110">CSV Return Type</span></span> | <span data-ttu-id="202fe-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="202fe-111">JSON Return Type</span></span>                         | <span data-ttu-id="202fe-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="202fe-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="202fe-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="202fe-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="202fe-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="202fe-114">Stream</span></span>          | [<span data-ttu-id="202fe-115">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="202fe-115">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="202fe-116">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="202fe-116">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="202fe-117">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="202fe-117">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="202fe-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="202fe-118">Stream</span></span>          | [<span data-ttu-id="202fe-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="202fe-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="202fe-120">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="202fe-120">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="202fe-121">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="202fe-121">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="202fe-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="202fe-122">Stream</span></span>          | [<span data-ttu-id="202fe-123">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="202fe-123">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="202fe-124">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="202fe-124">Get the trend in the number of active users.</span></span> <span data-ttu-id="202fe-125">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="202fe-125">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="202fe-126">Obter páginas</span><span class="sxs-lookup"><span data-stu-id="202fe-126">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="202fe-127">Fluxo</span><span class="sxs-lookup"><span data-stu-id="202fe-127">Stream</span></span>          | [<span data-ttu-id="202fe-128">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="202fe-128">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="202fe-129">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="202fe-129">Get the number of unique pages visited by users.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
