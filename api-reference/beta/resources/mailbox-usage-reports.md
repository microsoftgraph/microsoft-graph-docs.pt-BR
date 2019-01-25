---
title: Relatórios de uso da caixa de correio
description: Você pode obter informações sobre os usuários com uma caixa de correio e seus níveis de atividade que se basear principalmente nos emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: ac32d9c1a24726af95af3def0102484e6eaaffd4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528428"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="5bb9b-104">Relatórios de uso da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="5bb9b-104">Mailbox usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bb9b-105">Você pode obter informações sobre os usuários com uma caixa de correio e seus níveis de atividade que se basear principalmente nos emails enviados e recebidos.</span><span class="sxs-lookup"><span data-stu-id="5bb9b-105">You can get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="5bb9b-106">Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="5bb9b-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="5bb9b-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="5bb9b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="5bb9b-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="5bb9b-108">Reports</span></span>

| <span data-ttu-id="5bb9b-109">Função</span><span class="sxs-lookup"><span data-stu-id="5bb9b-109">Function</span></span>                                 | <span data-ttu-id="5bb9b-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="5bb9b-110">CSV return type</span></span> | <span data-ttu-id="5bb9b-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="5bb9b-111">JSON return type</span></span>                         | <span data-ttu-id="5bb9b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb9b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5bb9b-113">Obter dados de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="5bb9b-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="5bb9b-114">Stream</span><span class="sxs-lookup"><span data-stu-id="5bb9b-114">Stream</span></span>          | [<span data-ttu-id="5bb9b-115">mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="5bb9b-115">mailboxUsageDetail</span></span>](../resources/mailboxusagedetail.md) | <span data-ttu-id="5bb9b-116">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5bb9b-116">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="5bb9b-117">Obter contagens de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="5bb9b-117">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="5bb9b-118">Stream</span><span class="sxs-lookup"><span data-stu-id="5bb9b-118">Stream</span></span>          | [<span data-ttu-id="5bb9b-119">mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="5bb9b-119">mailboxUsageMailboxCounts</span></span>](../resources/mailboxusagemailboxcounts.md) | <span data-ttu-id="5bb9b-120">Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório.</span><span class="sxs-lookup"><span data-stu-id="5bb9b-120">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="5bb9b-121">Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.</span><span class="sxs-lookup"><span data-stu-id="5bb9b-121">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="5bb9b-122">Obter contagens da cota de status da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="5bb9b-122">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="5bb9b-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="5bb9b-123">Stream</span></span>          | [<span data-ttu-id="5bb9b-124">mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="5bb9b-124">mailboxUsageQuotaStatusMailboxCounts</span></span>](../resources/mailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="5bb9b-125">Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.</span><span class="sxs-lookup"><span data-stu-id="5bb9b-125">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="5bb9b-126">Obter armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bb9b-126">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="5bb9b-127">Stream</span><span class="sxs-lookup"><span data-stu-id="5bb9b-127">Stream</span></span>          | [<span data-ttu-id="5bb9b-128">mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="5bb9b-128">mailboxUsageStorage</span></span>](../resources/mailboxusagestorage.md) | <span data-ttu-id="5bb9b-129">Obtenha a quantidade de armazenamento usada em sua organização.</span><span class="sxs-lookup"><span data-stu-id="5bb9b-129">Get the amount of storage used in your organization.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailbox-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
