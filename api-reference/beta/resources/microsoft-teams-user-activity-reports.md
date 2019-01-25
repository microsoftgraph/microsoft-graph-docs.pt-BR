---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os relatórios de atividade do usuário Teams da Microsoft para obter ideias sobre a atividade do usuário Teams da Microsoft em sua organização.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 447aa9d36208ae9c966d86e733e99f81ab01e6ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517698"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="e18f5-103">Relatórios de atividades de usuários do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e18f5-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e18f5-104">Use os relatórios de atividade do usuário Teams da Microsoft para obter ideias sobre a atividade do usuário Teams da Microsoft em sua organização.</span><span class="sxs-lookup"><span data-stu-id="e18f5-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="e18f5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e18f5-105">Methods</span></span>

| <span data-ttu-id="e18f5-106">Método</span><span class="sxs-lookup"><span data-stu-id="e18f5-106">Method</span></span>                                   | <span data-ttu-id="e18f5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e18f5-107">Return Type</span></span>                              | <span data-ttu-id="e18f5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e18f5-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="e18f5-109">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="e18f5-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="e18f5-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e18f5-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="e18f5-111">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="e18f5-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="e18f5-112">Obter contagens de atividades</span><span class="sxs-lookup"><span data-stu-id="e18f5-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="e18f5-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="e18f5-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="e18f5-114">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="e18f5-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="e18f5-115">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="e18f5-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="e18f5-116">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="e18f5-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="e18f5-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e18f5-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="e18f5-118">Obtém o número de usuários por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="e18f5-118">Get the number of users by activity type.</span></span> <span data-ttu-id="e18f5-119">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="e18f5-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
