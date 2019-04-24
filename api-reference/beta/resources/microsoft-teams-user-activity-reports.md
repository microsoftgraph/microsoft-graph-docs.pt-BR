---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a071fb38ce9fd76aff4ccdc648201f91a600f24
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457078"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="9bdea-103">Relatórios de atividades de usuários do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9bdea-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bdea-104">Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.</span><span class="sxs-lookup"><span data-stu-id="9bdea-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="9bdea-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9bdea-105">Methods</span></span>

| <span data-ttu-id="9bdea-106">Método</span><span class="sxs-lookup"><span data-stu-id="9bdea-106">Method</span></span>                                   | <span data-ttu-id="9bdea-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9bdea-107">Return Type</span></span>                              | <span data-ttu-id="9bdea-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bdea-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="9bdea-109">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="9bdea-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="9bdea-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9bdea-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="9bdea-111">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="9bdea-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="9bdea-112">Obter contagens de atividades</span><span class="sxs-lookup"><span data-stu-id="9bdea-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="9bdea-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="9bdea-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="9bdea-114">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="9bdea-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="9bdea-115">Os tipos de atividade são número de mensagens de chat da equipe, mensagens de chat particular, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="9bdea-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="9bdea-116">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="9bdea-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="9bdea-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="9bdea-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="9bdea-118">Obtém o número de usuários por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="9bdea-118">Get the number of users by activity type.</span></span> <span data-ttu-id="9bdea-119">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="9bdea-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
