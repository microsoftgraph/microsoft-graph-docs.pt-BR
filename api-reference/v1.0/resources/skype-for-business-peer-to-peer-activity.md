---
title: Relatórios de atividades ponto a ponto Skype for Business
description: Você pode usar os relatórios de atividades ponto a ponto do Skype for Business para obter dados sobre as atividades ponto a ponto em toda a organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 5d967cd8a150d70598a98fd9019087472216a296
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970548"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a><span data-ttu-id="16d8b-104">Relatórios de atividades ponto a ponto Skype for Business</span><span class="sxs-lookup"><span data-stu-id="16d8b-104">Skype for Business peer-to-peer activity reports</span></span>

<span data-ttu-id="16d8b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16d8b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16d8b-106">Você pode usar os relatórios de atividades ponto a ponto do Skype for Business para obter dados sobre as atividades ponto a ponto em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="16d8b-106">You can use the Skype for Business peer-to-peer activity reports to get details on peer-to-peer activity across your organization.</span></span> <span data-ttu-id="16d8b-107">Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.</span><span class="sxs-lookup"><span data-stu-id="16d8b-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="16d8b-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Skype for Business peer-to-peer Activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="16d8b-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="reports"></a><span data-ttu-id="16d8b-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="16d8b-109">Reports</span></span>

| <span data-ttu-id="16d8b-110">Função</span><span class="sxs-lookup"><span data-stu-id="16d8b-110">Function</span></span>                                 | <span data-ttu-id="16d8b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="16d8b-111">Return Type</span></span> | <span data-ttu-id="16d8b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="16d8b-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="16d8b-113">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="16d8b-113">Get activity counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | <span data-ttu-id="16d8b-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="16d8b-114">Stream</span></span>      | <span data-ttu-id="16d8b-115">Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="16d8b-115">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="16d8b-116">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.</span><span class="sxs-lookup"><span data-stu-id="16d8b-116">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span> |
| [<span data-ttu-id="16d8b-117">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="16d8b-117">Get user counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | <span data-ttu-id="16d8b-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="16d8b-118">Stream</span></span>      | <span data-ttu-id="16d8b-119">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="16d8b-119">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="16d8b-120">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="16d8b-120">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="16d8b-121">Obter contagens de minutos</span><span class="sxs-lookup"><span data-stu-id="16d8b-121">Get minute counts</span></span>](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | <span data-ttu-id="16d8b-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="16d8b-122">Stream</span></span>      | <span data-ttu-id="16d8b-123">Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="16d8b-123">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="16d8b-124">Tipos de sessões incluem áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="16d8b-124">Types of sessions include audio and video.</span></span> |


