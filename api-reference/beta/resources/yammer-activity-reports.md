---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f46ea743aed25a40d0894a003a11eae49b2829d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046087"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="ce621-103">Relatórios de atividades do Yammer</span><span class="sxs-lookup"><span data-stu-id="ce621-103">Yammer activity reports</span></span>

<span data-ttu-id="ce621-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce621-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce621-105">Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.</span><span class="sxs-lookup"><span data-stu-id="ce621-105">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="ce621-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="ce621-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="ce621-107">Relatórios</span><span class="sxs-lookup"><span data-stu-id="ce621-107">Reports</span></span>

| <span data-ttu-id="ce621-108">Função</span><span class="sxs-lookup"><span data-stu-id="ce621-108">Function</span></span>                                 | <span data-ttu-id="ce621-109">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="ce621-109">CSV return type</span></span> | <span data-ttu-id="ce621-110">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="ce621-110">JSON return type</span></span>                         | <span data-ttu-id="ce621-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce621-111">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ce621-112">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="ce621-112">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="ce621-113">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ce621-113">Stream</span></span>          | [<span data-ttu-id="ce621-114">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ce621-114">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="ce621-115">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="ce621-115">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="ce621-116">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="ce621-116">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="ce621-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ce621-117">Stream</span></span>          | [<span data-ttu-id="ce621-118">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="ce621-118">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="ce621-119">Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.</span><span class="sxs-lookup"><span data-stu-id="ce621-119">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="ce621-120">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="ce621-120">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="ce621-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ce621-121">Stream</span></span>          | [<span data-ttu-id="ce621-122">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="ce621-122">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="ce621-123">Obtenha as tendências do número de usuários exclusivos que lançaram, ler e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="ce621-123">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |


