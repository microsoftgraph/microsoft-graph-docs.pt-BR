---
title: Relatórios de uso do OneDrive
description: Você pode obter uma visão de alto nível do valor que está obtendo do OneDrive em termos do número total de arquivos e armazenamento usados em todas as contas do OneDrive em sua organização. Você pode então detalhar as tendências das contas OneDrive ativas, quantos usuários de arquivos interagiram e quanto de armazenamento é usado. Também fornece os detalhes da conta do OneDrive.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 553dee26b757913c2d4f2186ce67f9c6f89b6fe3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897187"
---
# <a name="onedrive-usage-reports"></a>Relatórios de uso do OneDrive

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma visão de alto nível do valor que está obtendo do OneDrive em termos do número total de arquivos e armazenamento usados em todas as contas do OneDrive em sua organização. Você pode então detalhar as tendências das contas OneDrive ativas, quantos usuários de arquivos interagiram e quanto de armazenamento é usado. Também fornece os detalhes da conta do OneDrive.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do onedrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [Obter dados de conta](../api/reportroot-getonedriveusageaccountdetail.md) | Stream          | [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) | Obtenha dados sobre o uso do OneDrive por conta. |
| [Obter contagens de conta](../api/reportroot-getonedriveusageaccountcounts.md) | Fluxo          | [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) | Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveusagefilecounts.md) | Stream          | [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) | Obtenha o número total de arquivos em todos os sites e quantos são arquivos ativos. Um arquivo é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter armazenamento](../api/reportroot-getonedriveusagestorage.md) | Fluxo          | [siteUsageStorage](../resources/siteusagestorage.md) | Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business. |
