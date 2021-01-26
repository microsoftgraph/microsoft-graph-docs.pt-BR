---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível de envolvimento da sua organização com o Yammer pela quantidade de atividade gerada em toda a organização e pelo número de usuários exclusivos que postam, gostam e leem mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: c0009949b5eb429f15155059768365b201078134
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982464"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="e1aac-103">Relatórios de atividades do Yammer</span><span class="sxs-lookup"><span data-stu-id="e1aac-103">Yammer activity reports</span></span>

<span data-ttu-id="e1aac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1aac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1aac-105">Você pode entender o nível de envolvimento da sua organização com o Yammer pela quantidade de atividade gerada em toda a organização e pelo número de usuários exclusivos que postam, gostam e leem mensagens no Yammer.</span><span class="sxs-lookup"><span data-stu-id="e1aac-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="e1aac-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira [relatórios do Microsoft 365 - Atividade do Yammer.](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)</span><span class="sxs-lookup"><span data-stu-id="e1aac-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="e1aac-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="e1aac-107">Reports</span></span>

| <span data-ttu-id="e1aac-108">Função</span><span class="sxs-lookup"><span data-stu-id="e1aac-108">Function</span></span>                                 | <span data-ttu-id="e1aac-109">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="e1aac-109">CSV return type</span></span> | <span data-ttu-id="e1aac-110">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="e1aac-110">JSON return type</span></span>                         | <span data-ttu-id="e1aac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1aac-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="e1aac-112">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="e1aac-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="e1aac-113">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e1aac-113">Stream</span></span>          | [<span data-ttu-id="e1aac-114">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e1aac-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="e1aac-115">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="e1aac-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="e1aac-116">Obter contagens de atividades</span><span class="sxs-lookup"><span data-stu-id="e1aac-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="e1aac-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e1aac-117">Stream</span></span>          | [<span data-ttu-id="e1aac-118">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e1aac-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="e1aac-119">Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.</span><span class="sxs-lookup"><span data-stu-id="e1aac-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="e1aac-120">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="e1aac-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="e1aac-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e1aac-121">Stream</span></span>          | [<span data-ttu-id="e1aac-122">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="e1aac-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="e1aac-123">Veja as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="e1aac-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |


