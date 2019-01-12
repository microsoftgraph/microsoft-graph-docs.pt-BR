---
title: Relatórios de uso do site do SharePoint
description: Você pode obter uma visão de alto nível do valor que você está obtendo do SharePoint em termos o número total de arquivos que os usuários armazenam em sites do SharePoint, quantos arquivos ativamente estão sendo usados e o armazenamento consumidos entre todos esses sites. Em seguida, você pode analisar o relatório de uso do site do SharePoint para entender as tendências e por detalhes de nível de site para todos os sites.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 964ec64a2cbb15d639a619cf8debd5fb5875245e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950526"
---
# <a name="sharepoint-site-usage-reports"></a>Relatórios de uso do site do SharePoint

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode obter uma visão de alto nível do valor que você está obtendo do SharePoint em termos o número total de arquivos que os usuários armazenam em sites do SharePoint, quantos arquivos ativamente estão sendo usados e o armazenamento consumidos entre todos esses sites. Em seguida, você pode analisar o relatório de uso do site do SharePoint para entender as tendências e por detalhes de nível de site para todos os sites.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados do site](../api/reportroot-getsharepointsiteusagedetail.md) | Fluxo          | [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) | Obtenha dados sobre o uso do site do SharePoint. |
| [Obter contagens de arquivo](../api/reportroot-getsharepointsiteusagefilecounts.md) | Fluxo          | [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) | Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter contagens do site](../api/reportroot-getsharepointsiteusagesitecounts.md) | Fluxo          | [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) | Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter armazenamento](../api/reportroot-getsharepointsiteusagestorage.md) | Fluxo          | [siteUsageStorage](../resources/siteusagestorage.md) | Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório. |
| [Obter páginas](../api/reportroot-getsharepointsiteusagepages.md) | Fluxo          | [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) | Obtenha o número de páginas visualizadas em todos os sites. |
