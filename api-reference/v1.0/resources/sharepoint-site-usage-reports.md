---
title: Relatórios de uso do site do SharePoint
description: Você pode usar os relatórios de uso do site do SharePoint para obter uma visão de alto nível do valor que você obtém do SharePoint em termos do número total de arquivos que os usuários armazenam em sites do SharePoint, quantos arquivos estão sendo usados ativamente e o armazenamento consumido em todos esses sites. Então, você pode analisar esses relatórios para entender as tendências e os dados do nível do site para todos os sites.
localization_priority: Normal
ms.openlocfilehash: 0cef40040e20b7c7961f09166ca242f4e02f8579
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819870"
---
# <a name="sharepoint-site-usage-reports"></a>Relatórios de uso do site do SharePoint

Você pode usar os relatórios de uso do site do SharePoint para obter uma visão de alto nível do valor que você obtém do SharePoint em termos do número total de arquivos que os usuários armazenam em sites do SharePoint, quantos arquivos estão sendo usados ativamente e o armazenamento consumido em todos esses sites. Então, você pode analisar esses relatórios para entender as tendências e os dados do nível do site para todos os sites.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados do site](../api/reportroot-getsharepointsiteusagedetail.md) | Fluxo      | Obtenha dados sobre o uso do site do SharePoint. |
| [Obter contagens de arquivo](../api/reportroot-getsharepointsiteusagefilecounts.md) | Fluxo      | Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter contagens do site](../api/reportroot-getsharepointsiteusagesitecounts.md) | Fluxo      | Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter armazenamento](../api/reportroot-getsharepointsiteusagestorage.md) | Fluxo      | Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório. |
| [Obter páginas](../api/reportroot-getsharepointsiteusagepages.md) | Fluxo      | Obtenha o número de páginas visualizadas em todos os sites. |
