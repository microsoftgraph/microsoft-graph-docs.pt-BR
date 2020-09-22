---
title: Relatórios de uso do site do SharePoint
description: Você pode obter uma visão de alto nível do valor que você está obtendo do SharePoint em relação ao número total de arquivos que os usuários armazenam em sites do SharePoint, quantos arquivos estão sendo usados ativamente e o armazenamento consumido em todos esses sites. Em seguida, você pode analisar o relatório de uso do site do SharePoint para entender as tendências e os detalhes de acordo com o nível do site para todos os sites.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 7cb940fcbcfa611227c3289516e582f701e49803
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973670"
---
# <a name="sharepoint-site-usage-reports"></a>Relatórios de uso do site do SharePoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma visão de alto nível do valor que você está obtendo do SharePoint em relação ao número total de arquivos que os usuários armazenam em sites do SharePoint, quantos arquivos estão sendo usados ativamente e o armazenamento consumido em todos esses sites. Em seguida, você pode analisar o relatório de uso do site do SharePoint para entender as tendências e os detalhes de acordo com o nível do site para todos os sites.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados do site](../api/reportroot-getsharepointsiteusagedetail.md) | Fluxo          | [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) | Obtenha dados sobre o uso do site do SharePoint. |
| [Obter contagens de arquivo](../api/reportroot-getsharepointsiteusagefilecounts.md) | Fluxo          | [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) | Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter contagens do site](../api/reportroot-getsharepointsiteusagesitecounts.md) | Fluxo          | [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) | Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter armazenamento](../api/reportroot-getsharepointsiteusagestorage.md) | Fluxo          | [siteUsageStorage](../resources/siteusagestorage.md) | Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório. |
| [Obter páginas](../api/reportroot-getsharepointsiteusagepages.md) | Fluxo          | [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) | Obtenha o número de páginas visualizadas em todos os sites. |


