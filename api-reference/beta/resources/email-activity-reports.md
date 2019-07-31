---
title: Relatórios de atividades do email
description: Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios. Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 2540934b93a1047df5b19c4fe1b477ba30fd798c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972268"
---
# <a name="email-activity-reports"></a><span data-ttu-id="5173b-104">Relatórios de atividades do email</span><span class="sxs-lookup"><span data-stu-id="5173b-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5173b-105">Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios.</span><span class="sxs-lookup"><span data-stu-id="5173b-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="5173b-106">Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.</span><span class="sxs-lookup"><span data-stu-id="5173b-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="5173b-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="5173b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="5173b-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="5173b-108">Reports</span></span>

| <span data-ttu-id="5173b-109">Função</span><span class="sxs-lookup"><span data-stu-id="5173b-109">Function</span></span>                                 | <span data-ttu-id="5173b-110">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="5173b-110">CSV return type</span></span> | <span data-ttu-id="5173b-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="5173b-111">JSON return type</span></span>                         | <span data-ttu-id="5173b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5173b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5173b-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="5173b-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="5173b-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="5173b-114">Stream</span></span>          | [<span data-ttu-id="5173b-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="5173b-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="5173b-116">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="5173b-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="5173b-117">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="5173b-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="5173b-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="5173b-118">Stream</span></span>          | [<span data-ttu-id="5173b-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="5173b-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="5173b-120">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="5173b-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="5173b-121">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="5173b-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="5173b-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="5173b-122">Stream</span></span>          | [<span data-ttu-id="5173b-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="5173b-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="5173b-124">Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.</span><span class="sxs-lookup"><span data-stu-id="5173b-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
