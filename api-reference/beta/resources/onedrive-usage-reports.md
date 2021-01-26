---
title: Relatórios de uso do OneDrive
description: Você pode obter uma visão de alto nível do valor que está recebendo do OneDrive em termos do número total de arquivos e armazenamento usados em todas as contas do OneDrive em sua organização. Você pode então detalhar as tendências das contas OneDrive ativas, quantos usuários de arquivos interagiram e quanto de armazenamento é usado. Ele também fornece os detalhes por conta do OneDrive.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e1c6128fab80fb0b7a0ec1391f4022bb625b2442
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983199"
---
# <a name="onedrive-usage-reports"></a>Relatórios de uso do OneDrive

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma visão de alto nível do valor que está recebendo do OneDrive em termos do número total de arquivos e armazenamento usados em todas as contas do OneDrive em sua organização. Você pode então detalhar as tendências das contas OneDrive ativas, quantos usuários de arquivos interagiram e quanto de armazenamento é usado. Ele também fornece os detalhes por conta do OneDrive.

> **Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira relatórios do [Microsoft 365 - uso do OneDrive for Business.](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [Obter dados de conta](../api/reportroot-getonedriveusageaccountdetail.md) | Fluxo          | [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) | Obtenha dados sobre o uso do OneDrive por conta. |
| [Obter contagens de conta](../api/reportroot-getonedriveusageaccountcounts.md) | Fluxo          | [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) | Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveusagefilecounts.md) | Fluxo          | [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) | Obtenha o número total de arquivos em todos os sites e quantos são arquivos ativos. Um arquivo é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter armazenamento](../api/reportroot-getonedriveusagestorage.md) | Fluxo          | [siteUsageStorage](../resources/siteusagestorage.md) | Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business. |


