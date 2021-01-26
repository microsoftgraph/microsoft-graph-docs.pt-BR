---
title: Relatórios de atividades do Skype for Business
description: Você pode obter detalhes sobre as atividades em toda a organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 0fe3236fc8c4f29357e2ae3fae45c80969c353db
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980644"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="9a623-104">Relatórios de atividades do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="9a623-104">Skype for Business activity reports</span></span>

<span data-ttu-id="9a623-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a623-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a623-106">Você pode obter detalhes sobre as atividades em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="9a623-106">You can get details on activity across your organization.</span></span> <span data-ttu-id="9a623-107">Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.</span><span class="sxs-lookup"><span data-stu-id="9a623-107">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="9a623-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="9a623-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="9a623-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="9a623-109">Reports</span></span>

| <span data-ttu-id="9a623-110">Função</span><span class="sxs-lookup"><span data-stu-id="9a623-110">Function</span></span>                                 | <span data-ttu-id="9a623-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="9a623-111">CSV return type</span></span> | <span data-ttu-id="9a623-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="9a623-112">JSON return type</span></span>                         | <span data-ttu-id="9a623-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a623-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="9a623-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="9a623-114">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="9a623-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9a623-115">Stream</span></span>          | [<span data-ttu-id="9a623-116">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9a623-116">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="9a623-117">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="9a623-117">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="9a623-118">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="9a623-118">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="9a623-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9a623-119">Stream</span></span>          | [<span data-ttu-id="9a623-120">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="9a623-120">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="9a623-121">Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="9a623-121">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="9a623-122">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="9a623-122">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="9a623-123">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="9a623-123">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="9a623-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9a623-124">Stream</span></span>          | [<span data-ttu-id="9a623-125">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="9a623-125">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="9a623-126">Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="9a623-126">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="9a623-127">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="9a623-127">The report also includes the number of peer-to-peer sessions.</span></span> |


