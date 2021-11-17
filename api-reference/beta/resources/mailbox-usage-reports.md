---
title: Relatórios de uso da caixa de correio
description: Você pode obter informações sobre usuários com uma caixa de correio e seu nível de atividade que se baseia principalmente em emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.
ms.localizationpriority: medium
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: a6645a6952c2fe21cc2e7e323dccb61cc43e36b2
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044747"
---
# <a name="mailbox-usage-reports"></a>Relatórios de uso da caixa de correio

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter informações sobre usuários com uma caixa de correio e seu nível de atividade que se baseia principalmente em emails enviados e recebidos. Você também pode conferir a quantidade de armazenamento que cada caixa postal consome e quantas caixas de correio estão se aproximando das cotas de armazenamento.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados de caixa de correio](../api/reportroot-getmailboxusagedetail.md) | Fluxo          | Fluxo           | Obtenha dados sobre o uso da caixa de correio.                             |
| [Obter contagens de caixa de correio](../api/reportroot-getmailboxusagemailboxcounts.md) | Fluxo          | Fluxo           | Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório. Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email. |
| [Obter contagens da cota de status da caixa de correio](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Fluxo          | Fluxo           | Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.      |
| [Obter armazenamento](../api/reportroot-getmailboxusagestorage.md)   | Fluxo          | Fluxo           | Obtenha a quantidade de armazenamento usada em sua organização.         |


