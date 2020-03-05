---
title: Relatórios de atividades do email
description: Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios. Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 7dcfaf2d5cc2d1dbd38cdc4a8a7c5eac71e9539b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499803"
---
# <a name="email-activity-reports"></a><span data-ttu-id="ba16b-104">Relatórios de atividades do email</span><span class="sxs-lookup"><span data-stu-id="ba16b-104">Email activity reports</span></span>

<span data-ttu-id="ba16b-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ba16b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba16b-106">Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios.</span><span class="sxs-lookup"><span data-stu-id="ba16b-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="ba16b-107">Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.</span><span class="sxs-lookup"><span data-stu-id="ba16b-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="ba16b-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="ba16b-108">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="ba16b-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="ba16b-109">Reports</span></span>

| <span data-ttu-id="ba16b-110">Função</span><span class="sxs-lookup"><span data-stu-id="ba16b-110">Function</span></span>                                 | <span data-ttu-id="ba16b-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="ba16b-111">CSV return type</span></span> | <span data-ttu-id="ba16b-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="ba16b-112">JSON return type</span></span>                         | <span data-ttu-id="ba16b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba16b-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ba16b-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="ba16b-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="ba16b-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ba16b-115">Stream</span></span>          | [<span data-ttu-id="ba16b-116">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ba16b-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="ba16b-117">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="ba16b-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="ba16b-118">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="ba16b-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="ba16b-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ba16b-119">Stream</span></span>          | [<span data-ttu-id="ba16b-120">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="ba16b-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="ba16b-121">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="ba16b-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="ba16b-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="ba16b-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="ba16b-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ba16b-123">Stream</span></span>          | [<span data-ttu-id="ba16b-124">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="ba16b-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="ba16b-125">Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.</span><span class="sxs-lookup"><span data-stu-id="ba16b-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
