---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 8f1358c188b06953d7af180c2b7ad83b6183af35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519054"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="678ce-103">Relatórios de atividades do Yammer</span><span class="sxs-lookup"><span data-stu-id="678ce-103">Yammer activity reports</span></span>

<span data-ttu-id="678ce-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="678ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="678ce-105">Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.</span><span class="sxs-lookup"><span data-stu-id="678ce-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="678ce-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="678ce-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="678ce-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="678ce-107">Reports</span></span>

| <span data-ttu-id="678ce-108">Função</span><span class="sxs-lookup"><span data-stu-id="678ce-108">Function</span></span>                                 | <span data-ttu-id="678ce-109">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="678ce-109">CSV return type</span></span> | <span data-ttu-id="678ce-110">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="678ce-110">JSON return type</span></span>                         | <span data-ttu-id="678ce-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="678ce-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="678ce-112">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="678ce-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="678ce-113">Stream</span><span class="sxs-lookup"><span data-stu-id="678ce-113">Stream</span></span>          | [<span data-ttu-id="678ce-114">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="678ce-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="678ce-115">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="678ce-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="678ce-116">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="678ce-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="678ce-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="678ce-117">Stream</span></span>          | [<span data-ttu-id="678ce-118">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="678ce-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="678ce-119">Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.</span><span class="sxs-lookup"><span data-stu-id="678ce-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="678ce-120">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="678ce-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="678ce-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="678ce-121">Stream</span></span>          | [<span data-ttu-id="678ce-122">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="678ce-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="678ce-123">Obtenha as tendências do número de usuários exclusivos que lançaram, ler e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="678ce-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
