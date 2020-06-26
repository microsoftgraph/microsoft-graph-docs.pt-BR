---
title: Relatórios de uso da caixa de correio
description: Você pode obter informações sobre os usuários com uma caixa de correio e seu nível de atividade, que baseia-se principalmente nos emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 7839860763fedf1a8eaeca8a98a7930f6d2a72fc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897040"
---
# <a name="mailbox-usage-reports"></a>Relatórios de uso da caixa de correio

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter informações sobre os usuários com uma caixa de correio e seu nível de atividade, que baseia-se principalmente nos emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Mailbox Usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de caixa de correio](../api/reportroot-getmailboxusagedetail.md) | Stream          | [mailboxUsageDetail](../resources/mailboxusagedetail.md) | Obtenha dados sobre o uso da caixa de correio.         |
| [Obter contagens de caixa de correio](../api/reportroot-getmailboxusagemailboxcounts.md) | Fluxo          | [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) | Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório. Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email. |
| [Obter contagens da cota de status da caixa de correio](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Fluxo          | [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) | Obtenha a contagem de caixas de correio de usuário em cada categoria de cota. |
| [Obter armazenamento](../api/reportroot-getmailboxusagestorage.md) | Fluxo          | [mailboxUsageStorage](../resources/mailboxusagestorage.md) | Obtenha a quantidade de armazenamento usada em sua organização. |
