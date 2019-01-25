---
title: Relatórios de atividades do Skype for Business
description: Você pode obter detalhes sobre a atividade em toda a organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a81e27d58316cb415d6296b4f77519a3f2125643
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512392"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="4107b-104">Relatórios de atividades do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="4107b-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4107b-105">Você pode obter detalhes sobre a atividade em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="4107b-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="4107b-106">Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.</span><span class="sxs-lookup"><span data-stu-id="4107b-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="4107b-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="4107b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="4107b-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="4107b-108">Reports</span></span>

| <span data-ttu-id="4107b-109">Função</span><span class="sxs-lookup"><span data-stu-id="4107b-109">Function</span></span>                                 | <span data-ttu-id="4107b-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="4107b-110">CSV return type</span></span> | <span data-ttu-id="4107b-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="4107b-111">JSON return type</span></span>                         | <span data-ttu-id="4107b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4107b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="4107b-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="4107b-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="4107b-114">Stream</span><span class="sxs-lookup"><span data-stu-id="4107b-114">Stream</span></span>          | [<span data-ttu-id="4107b-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4107b-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="4107b-116">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="4107b-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="4107b-117">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="4107b-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="4107b-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="4107b-118">Stream</span></span>          | [<span data-ttu-id="4107b-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4107b-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="4107b-120">Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="4107b-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="4107b-121">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="4107b-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="4107b-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="4107b-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="4107b-123">Stream</span><span class="sxs-lookup"><span data-stu-id="4107b-123">Stream</span></span>          | [<span data-ttu-id="4107b-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="4107b-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="4107b-125">Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="4107b-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="4107b-126">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="4107b-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
