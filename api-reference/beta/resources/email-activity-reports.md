---
title: Relatórios de atividades do email
description: Você pode obter um modo de exibição de alto nível de tráfego de email dentro da sua organização a partir da página de relatórios. Você também pode analisar o widget da atividade de Email para entender as tendências e detalhes por usuário da atividade de email na sua organização.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 748199a2e846cc71a3f04c3ea1bda97dcf2c7301
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573897"
---
# <a name="email-activity-reports"></a><span data-ttu-id="714f6-104">Relatórios de atividades do email</span><span class="sxs-lookup"><span data-stu-id="714f6-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="714f6-105">Você pode obter um modo de exibição de alto nível de tráfego de email dentro da sua organização a partir da página de relatórios.</span><span class="sxs-lookup"><span data-stu-id="714f6-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="714f6-106">Você também pode analisar o widget da atividade de Email para entender as tendências e detalhes por usuário da atividade de email na sua organização.</span><span class="sxs-lookup"><span data-stu-id="714f6-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="714f6-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="714f6-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="714f6-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="714f6-108">Reports</span></span>

| <span data-ttu-id="714f6-109">Função</span><span class="sxs-lookup"><span data-stu-id="714f6-109">Function</span></span>                                 | <span data-ttu-id="714f6-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="714f6-110">CSV return type</span></span> | <span data-ttu-id="714f6-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="714f6-111">JSON return type</span></span>                         | <span data-ttu-id="714f6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="714f6-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="714f6-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="714f6-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="714f6-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="714f6-114">Stream</span></span>          | [<span data-ttu-id="714f6-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="714f6-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="714f6-116">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="714f6-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="714f6-117">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="714f6-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="714f6-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="714f6-118">Stream</span></span>          | [<span data-ttu-id="714f6-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="714f6-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="714f6-120">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="714f6-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="714f6-121">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="714f6-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="714f6-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="714f6-122">Stream</span></span>          | [<span data-ttu-id="714f6-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="714f6-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="714f6-124">Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.</span><span class="sxs-lookup"><span data-stu-id="714f6-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
