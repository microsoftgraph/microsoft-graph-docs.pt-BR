---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ca8d1f772744b33aa5fee60fc3b843bf60b0be9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009633"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="275be-103">Relatórios de atividades de usuários do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="275be-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="275be-104">Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.</span><span class="sxs-lookup"><span data-stu-id="275be-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="275be-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="275be-105">Methods</span></span>

| <span data-ttu-id="275be-106">Método</span><span class="sxs-lookup"><span data-stu-id="275be-106">Method</span></span>                                   | <span data-ttu-id="275be-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="275be-107">Return Type</span></span>                              | <span data-ttu-id="275be-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="275be-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="275be-109">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="275be-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="275be-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="275be-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="275be-111">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="275be-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="275be-112">Obter contagens de atividades</span><span class="sxs-lookup"><span data-stu-id="275be-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="275be-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="275be-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="275be-114">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="275be-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="275be-115">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="275be-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="275be-116">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="275be-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="275be-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="275be-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="275be-118">Obtém o número de usuários por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="275be-118">Get the number of users by activity type.</span></span> <span data-ttu-id="275be-119">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="275be-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
