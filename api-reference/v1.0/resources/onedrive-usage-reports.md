---
title: Relatórios de uso do OneDrive
description: Você pode usar os relatórios de uso do OneDrive para obter uma visão de alto nível do valor que você obteve do OneDrive em termos do número total de arquivos e armazenamento usados em todas as contas OneDrive da sua organização. Você pode então detalhar as tendências das contas OneDrive ativas, quantos usuários de arquivos interagiram e quanto de armazenamento é usado. Esses relatórios também podem fornecer dados sobre a conta do OneDrive.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: fdcf1eb277733da2ea46a30fb9985ea889ae87ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962664"
---
# <a name="onedrive-usage-reports"></a>Relatórios de uso do OneDrive

Você pode usar os relatórios de uso do OneDrive para obter uma visão de alto nível do valor que você obteve do OneDrive em termos do número total de arquivos e armazenamento usados em todas as contas OneDrive da sua organização. Você pode então detalhar as tendências das contas OneDrive ativas, quantos usuários de arquivos interagiram e quanto de armazenamento é usado. Esses relatórios também podem fornecer dados sobre a conta do OneDrive.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | ---------------------------------------- |
| [Obter dados de conta](../api/reportroot-getonedriveusageaccountdetail.md) | Fluxo      | Obtenha dados sobre o uso do OneDrive por conta. |
| [Obter contagens de conta](../api/reportroot-getonedriveusageaccountcounts.md) | Fluxo      | Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveusagefilecounts.md) | Fluxo      | Obtenha o número total de arquivos em todos os sites e quantos são arquivos ativos. Um arquivo é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter armazenamento](../api/reportroot-getonedriveusagestorage.md) | Fluxo      | Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business. |
