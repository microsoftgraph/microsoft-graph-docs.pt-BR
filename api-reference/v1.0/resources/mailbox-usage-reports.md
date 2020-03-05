---
title: Relatórios de uso da caixa de correio
description: Use os relatórios de uso da caixa de correio para obter informações sobre usuários com uma caixa de correio e seu nível de atividade, que é principalmente baseado em emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 3c7b932bf7f0747ff6b5050f7e19accf871c1b1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447511"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="97cd7-104">Relatórios de uso da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="97cd7-104">Mailbox usage reports</span></span>

<span data-ttu-id="97cd7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97cd7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97cd7-106">Use os relatórios de uso da caixa de correio para obter informações sobre usuários com uma caixa de correio e seu nível de atividade, que é principalmente baseado em emails enviados e recebidos.</span><span class="sxs-lookup"><span data-stu-id="97cd7-106">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="97cd7-107">Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="97cd7-107">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="97cd7-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="97cd7-108">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="97cd7-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="97cd7-109">Reports</span></span>

| <span data-ttu-id="97cd7-110">Função</span><span class="sxs-lookup"><span data-stu-id="97cd7-110">Function</span></span>                                 | <span data-ttu-id="97cd7-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="97cd7-111">Return Type</span></span> | <span data-ttu-id="97cd7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="97cd7-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="97cd7-113">Obter dados de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="97cd7-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="97cd7-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="97cd7-114">Stream</span></span>      | <span data-ttu-id="97cd7-115">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="97cd7-115">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="97cd7-116">Obter contagens de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="97cd7-116">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="97cd7-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="97cd7-117">Stream</span></span>      | <span data-ttu-id="97cd7-118">Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório.</span><span class="sxs-lookup"><span data-stu-id="97cd7-118">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="97cd7-119">Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.</span><span class="sxs-lookup"><span data-stu-id="97cd7-119">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="97cd7-120">Obter contagens da cota de status da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="97cd7-120">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="97cd7-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="97cd7-121">Stream</span></span>      | <span data-ttu-id="97cd7-122">Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.</span><span class="sxs-lookup"><span data-stu-id="97cd7-122">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="97cd7-123">Obter armazenamento</span><span class="sxs-lookup"><span data-stu-id="97cd7-123">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="97cd7-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="97cd7-124">Stream</span></span>      | <span data-ttu-id="97cd7-125">Obtenha a quantidade de armazenamento usada em sua organização.</span><span class="sxs-lookup"><span data-stu-id="97cd7-125">Get the amount of storage used in your organization.</span></span> |
