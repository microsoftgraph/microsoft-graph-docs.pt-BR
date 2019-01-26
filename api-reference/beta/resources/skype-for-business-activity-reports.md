---
title: Relatórios de atividades do Skype for Business
description: Você pode obter detalhes sobre a atividade em toda a organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577379"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="ac918-104">Relatórios de atividades do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="ac918-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac918-105">Você pode obter detalhes sobre a atividade em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="ac918-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="ac918-106">Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.</span><span class="sxs-lookup"><span data-stu-id="ac918-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="ac918-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="ac918-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="ac918-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="ac918-108">Reports</span></span>

| <span data-ttu-id="ac918-109">Função</span><span class="sxs-lookup"><span data-stu-id="ac918-109">Function</span></span>                                 | <span data-ttu-id="ac918-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="ac918-110">CSV return type</span></span> | <span data-ttu-id="ac918-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="ac918-111">JSON return type</span></span>                         | <span data-ttu-id="ac918-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac918-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ac918-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="ac918-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="ac918-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ac918-114">Stream</span></span>          | [<span data-ttu-id="ac918-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ac918-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="ac918-116">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="ac918-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="ac918-117">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="ac918-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="ac918-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ac918-118">Stream</span></span>          | [<span data-ttu-id="ac918-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ac918-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="ac918-120">Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="ac918-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="ac918-121">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="ac918-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="ac918-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="ac918-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="ac918-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ac918-123">Stream</span></span>          | [<span data-ttu-id="ac918-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ac918-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="ac918-125">Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="ac918-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="ac918-126">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="ac918-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
