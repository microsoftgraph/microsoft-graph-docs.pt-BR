---
title: Relatórios de atividades do email
description: Você pode obter uma visão de alto nível do tráfego de email em sua organização na página Relatórios. Você também pode detalhar o widget Atividade de Email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: db9ea032b418a6beca7afb7c15eb16b762e6ed11
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983794"
---
# <a name="email-activity-reports"></a><span data-ttu-id="039d6-104">Relatórios de atividades do email</span><span class="sxs-lookup"><span data-stu-id="039d6-104">Email activity reports</span></span>

<span data-ttu-id="039d6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="039d6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="039d6-106">Você pode obter uma visão de alto nível do tráfego de email em sua organização na página Relatórios.</span><span class="sxs-lookup"><span data-stu-id="039d6-106">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="039d6-107">Você também pode detalhar o widget Atividade de Email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.</span><span class="sxs-lookup"><span data-stu-id="039d6-107">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="039d6-108">**Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Atividade de E-mail](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="039d6-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="039d6-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="039d6-109">Reports</span></span>

| <span data-ttu-id="039d6-110">Função</span><span class="sxs-lookup"><span data-stu-id="039d6-110">Function</span></span>                                 | <span data-ttu-id="039d6-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="039d6-111">CSV return type</span></span> | <span data-ttu-id="039d6-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="039d6-112">JSON return type</span></span>                         | <span data-ttu-id="039d6-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="039d6-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="039d6-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="039d6-114">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="039d6-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="039d6-115">Stream</span></span>          | [<span data-ttu-id="039d6-116">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="039d6-116">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="039d6-117">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="039d6-117">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="039d6-118">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="039d6-118">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="039d6-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="039d6-119">Stream</span></span>          | [<span data-ttu-id="039d6-120">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="039d6-120">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="039d6-121">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="039d6-121">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="039d6-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="039d6-122">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="039d6-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="039d6-123">Stream</span></span>          | [<span data-ttu-id="039d6-124">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="039d6-124">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="039d6-125">Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.</span><span class="sxs-lookup"><span data-stu-id="039d6-125">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |


