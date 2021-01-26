---
title: Relatórios de uso da caixa de correio
description: Use os relatórios de uso da caixa de correio para obter informações sobre usuários com uma caixa de correio e seu nível de atividade, que é principalmente baseado em emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.
localization_priority: Priority
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: d460f2c72878065abdd1df2fa58dc0eb8f4d411b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981113"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="eec9f-104">Relatórios de uso da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="eec9f-104">Mailbox usage reports</span></span>

<span data-ttu-id="eec9f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eec9f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eec9f-106">Use os relatórios de uso da caixa de correio para obter informações sobre usuários com uma caixa de correio e seu nível de atividade, que é principalmente baseado em emails enviados e recebidos.</span><span class="sxs-lookup"><span data-stu-id="eec9f-106">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="eec9f-107">Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="eec9f-107">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="eec9f-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="eec9f-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="eec9f-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="eec9f-109">Reports</span></span>

| <span data-ttu-id="eec9f-110">Função</span><span class="sxs-lookup"><span data-stu-id="eec9f-110">Function</span></span>                                 | <span data-ttu-id="eec9f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eec9f-111">Return Type</span></span> | <span data-ttu-id="eec9f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="eec9f-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="eec9f-113">Obter dados de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="eec9f-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="eec9f-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="eec9f-114">Stream</span></span>      | <span data-ttu-id="eec9f-115">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="eec9f-115">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="eec9f-116">Obter contagens de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="eec9f-116">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="eec9f-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="eec9f-117">Stream</span></span>      | <span data-ttu-id="eec9f-118">Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório.</span><span class="sxs-lookup"><span data-stu-id="eec9f-118">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="eec9f-119">Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.</span><span class="sxs-lookup"><span data-stu-id="eec9f-119">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="eec9f-120">Obter contagens da cota de status da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="eec9f-120">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="eec9f-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="eec9f-121">Stream</span></span>      | <span data-ttu-id="eec9f-122">Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.</span><span class="sxs-lookup"><span data-stu-id="eec9f-122">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="eec9f-123">Obter armazenamento</span><span class="sxs-lookup"><span data-stu-id="eec9f-123">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="eec9f-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="eec9f-124">Stream</span></span>      | <span data-ttu-id="eec9f-125">Obtenha a quantidade de armazenamento usada em sua organização.</span><span class="sxs-lookup"><span data-stu-id="eec9f-125">Get the amount of storage used in your organization.</span></span> |

