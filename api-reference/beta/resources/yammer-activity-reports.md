---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 6c431bf8bd72d2afb380d13c3cef310c2b1e672e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897082"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="6198c-103">Relatórios de atividades do Yammer</span><span class="sxs-lookup"><span data-stu-id="6198c-103">Yammer activity reports</span></span>

<span data-ttu-id="6198c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6198c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6198c-105">Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.</span><span class="sxs-lookup"><span data-stu-id="6198c-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="6198c-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="6198c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="6198c-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="6198c-107">Reports</span></span>

| <span data-ttu-id="6198c-108">Função</span><span class="sxs-lookup"><span data-stu-id="6198c-108">Function</span></span>                                 | <span data-ttu-id="6198c-109">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="6198c-109">CSV return type</span></span> | <span data-ttu-id="6198c-110">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="6198c-110">JSON return type</span></span>                         | <span data-ttu-id="6198c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6198c-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="6198c-112">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="6198c-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="6198c-113">Stream</span><span class="sxs-lookup"><span data-stu-id="6198c-113">Stream</span></span>          | [<span data-ttu-id="6198c-114">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="6198c-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="6198c-115">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="6198c-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="6198c-116">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="6198c-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="6198c-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="6198c-117">Stream</span></span>          | [<span data-ttu-id="6198c-118">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="6198c-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="6198c-119">Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.</span><span class="sxs-lookup"><span data-stu-id="6198c-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="6198c-120">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="6198c-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="6198c-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="6198c-121">Stream</span></span>          | [<span data-ttu-id="6198c-122">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="6198c-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="6198c-123">Obtenha as tendências do número de usuários exclusivos que lançaram, ler e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="6198c-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
