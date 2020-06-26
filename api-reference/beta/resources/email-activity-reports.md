---
title: Relatórios de atividades do email
description: Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios. Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 5f26498a0837993fc052cb536acd8bcd08f77ee1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896907"
---
# <a name="email-activity-reports"></a><span data-ttu-id="d2570-104">Relatórios de atividades do email</span><span class="sxs-lookup"><span data-stu-id="d2570-104">Email activity reports</span></span>

<span data-ttu-id="d2570-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2570-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2570-106">Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios.</span><span class="sxs-lookup"><span data-stu-id="d2570-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="d2570-107">Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d2570-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="d2570-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-E-mail Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="d2570-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="d2570-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="d2570-109">Reports</span></span>

| <span data-ttu-id="d2570-110">Função</span><span class="sxs-lookup"><span data-stu-id="d2570-110">Function</span></span>                                 | <span data-ttu-id="d2570-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="d2570-111">CSV return type</span></span> | <span data-ttu-id="d2570-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="d2570-112">JSON return type</span></span>                         | <span data-ttu-id="d2570-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2570-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d2570-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="d2570-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="d2570-115">Stream</span><span class="sxs-lookup"><span data-stu-id="d2570-115">Stream</span></span>          | [<span data-ttu-id="d2570-116">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d2570-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="d2570-117">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="d2570-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="d2570-118">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="d2570-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="d2570-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="d2570-119">Stream</span></span>          | [<span data-ttu-id="d2570-120">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="d2570-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="d2570-121">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d2570-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="d2570-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="d2570-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="d2570-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="d2570-123">Stream</span></span>          | [<span data-ttu-id="d2570-124">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="d2570-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="d2570-125">Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.</span><span class="sxs-lookup"><span data-stu-id="d2570-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
