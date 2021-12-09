---
title: Relatórios de uso do OneDrive
description: Você pode obter uma exibição de alto nível do valor que você está recebendo do OneDrive em termos do número total de arquivos e armazenamento usados em todas as contas OneDrive de sua organização. Você pode então detalhar as tendências das contas OneDrive ativas, quantos usuários de arquivos interagiram e quanto de armazenamento é usado. Ele também fornece os detalhes por OneDrive conta.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 6219126a872af35d2c6a2f757e80ebe440ed8898
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390680"
---
# <a name="onedrive-usage-reports"></a>Relatórios de uso do OneDrive

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma exibição de alto nível do valor que você está recebendo do OneDrive em termos do número total de arquivos e armazenamento usados em todas as contas OneDrive de sua organização. Você pode então detalhar as tendências das contas OneDrive ativas, quantos usuários de arquivos interagiram e quanto de armazenamento é usado. Ele também fornece os detalhes por OneDrive conta.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - OneDrive for Business uso](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | ---------------- | ------------------------------------------------------------ |
| [Obter dados de conta](../api/reportroot-getonedriveusageaccountdetail.md) | Fluxo          | Fluxo           | Obtenha dados sobre o uso do OneDrive por conta.                 |
| [Obter contagens de conta](../api/reportroot-getonedriveusageaccountcounts.md) | Fluxo          | Fluxo           | Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveusagefilecounts.md) | Fluxo          | Fluxo           | Obtenha o número total de arquivos em todos os sites e quantos são arquivos ativos. Um arquivo é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter armazenamento](../api/reportroot-getonedriveusagestorage.md)  | Fluxo          | Fluxo           | Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business. |


