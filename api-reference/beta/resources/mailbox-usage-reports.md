---
title: Relatórios de uso da caixa de correio
description: Você pode obter informações sobre os usuários com uma caixa de correio e seu nível de atividade, que baseia-se principalmente nos emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: f3942bc4dc0eebb66a8ec0b9a8fc08619089c264
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095014"
---
# <a name="mailbox-usage-reports"></a>Relatórios de uso da caixa de correio

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter informações sobre os usuários com uma caixa de correio e seu nível de atividade, que baseia-se principalmente nos emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Mailbox Usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de caixa de correio](../api/reportroot-getmailboxusagedetail.md) | Fluxo          | [mailboxUsageDetail](../resources/mailboxusagedetail.md) | Obtenha dados sobre o uso da caixa de correio.         |
| [Obter contagens de caixa de correio](../api/reportroot-getmailboxusagemailboxcounts.md) | Fluxo          | [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) | Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório. Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email. |
| [Obter contagens da cota de status da caixa de correio](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Fluxo          | [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) | Obtenha a contagem de caixas de correio de usuário em cada categoria de cota. |
| [Obter armazenamento](../api/reportroot-getmailboxusagestorage.md) | Fluxo          | [mailboxUsageStorage](../resources/mailboxusagestorage.md) | Obtenha a quantidade de armazenamento usada em sua organização. |


