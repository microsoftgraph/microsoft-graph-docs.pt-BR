---
title: Relatórios de uso da caixa de correio
description: Use os relatórios de uso da caixa de correio para obter informações sobre usuários com uma caixa de correio e seu nível de atividade, que é principalmente baseado em emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.
localization_priority: Priority
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 6b02821da78338e8af1dec99fe73bedf81561116
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574086"
---
# <a name="mailbox-usage-reports"></a>Relatórios de uso da caixa de correio

Use os relatórios de uso da caixa de correio para obter informações sobre usuários com uma caixa de correio e seu nível de atividade, que é principalmente baseado em emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de caixa de correio](../api/reportroot-getmailboxusagedetail.md) | Fluxo      | Obtenha dados sobre o uso da caixa de correio.         |
| [Obter contagens de caixa de correio](../api/reportroot-getmailboxusagemailboxcounts.md) | Fluxo      | Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório. Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email. |
| [Obter contagens da cota de status da caixa de correio](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Fluxo      | Obtenha a contagem de caixas de correio de usuário em cada categoria de cota. |
| [Obter armazenamento](../api/reportroot-getmailboxusagestorage.md) | Fluxo      | Obtenha a quantidade de armazenamento usada em sua organização. |
