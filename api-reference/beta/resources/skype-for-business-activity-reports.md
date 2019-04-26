---
title: Relatórios de atividades do Skype for Business
description: Você pode obter detalhes sobre a atividade em sua organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551901"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="64a98-104">Relatórios de atividades do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="64a98-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64a98-105">Você pode obter detalhes sobre a atividade em sua organização.</span><span class="sxs-lookup"><span data-stu-id="64a98-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="64a98-106">Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.</span><span class="sxs-lookup"><span data-stu-id="64a98-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="64a98-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="64a98-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="64a98-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="64a98-108">Reports</span></span>

| <span data-ttu-id="64a98-109">Função</span><span class="sxs-lookup"><span data-stu-id="64a98-109">Function</span></span>                                 | <span data-ttu-id="64a98-110">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="64a98-110">CSV return type</span></span> | <span data-ttu-id="64a98-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="64a98-111">JSON return type</span></span>                         | <span data-ttu-id="64a98-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="64a98-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="64a98-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="64a98-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="64a98-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="64a98-114">Stream</span></span>          | [<span data-ttu-id="64a98-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="64a98-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="64a98-116">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="64a98-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="64a98-117">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="64a98-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="64a98-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="64a98-118">Stream</span></span>          | [<span data-ttu-id="64a98-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="64a98-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="64a98-120">Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="64a98-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="64a98-121">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="64a98-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="64a98-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="64a98-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="64a98-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="64a98-123">Stream</span></span>          | [<span data-ttu-id="64a98-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="64a98-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="64a98-125">Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="64a98-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="64a98-126">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="64a98-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
