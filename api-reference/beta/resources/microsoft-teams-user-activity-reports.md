---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: c5807af05bda74019ac8b28c53f902ecac6f8e2a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522628"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="7f1f9-103">Relatórios de atividades de usuários do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7f1f9-103">Microsoft Teams user activity reports</span></span>

<span data-ttu-id="7f1f9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7f1f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f1f9-105">Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.</span><span class="sxs-lookup"><span data-stu-id="7f1f9-105">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="7f1f9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7f1f9-106">Methods</span></span>

| <span data-ttu-id="7f1f9-107">Método</span><span class="sxs-lookup"><span data-stu-id="7f1f9-107">Method</span></span>                                   | <span data-ttu-id="7f1f9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f1f9-108">Return Type</span></span>                              | <span data-ttu-id="7f1f9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f1f9-109">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="7f1f9-110">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="7f1f9-110">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="7f1f9-111">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7f1f9-111">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="7f1f9-112">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="7f1f9-112">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="7f1f9-113">Obter contagens de atividades</span><span class="sxs-lookup"><span data-stu-id="7f1f9-113">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="7f1f9-114">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="7f1f9-114">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="7f1f9-115">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="7f1f9-115">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="7f1f9-116">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="7f1f9-116">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="7f1f9-117">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="7f1f9-117">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="7f1f9-118">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7f1f9-118">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="7f1f9-119">Obtém o número de usuários por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="7f1f9-119">Get the number of users by activity type.</span></span> <span data-ttu-id="7f1f9-120">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="7f1f9-120">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
