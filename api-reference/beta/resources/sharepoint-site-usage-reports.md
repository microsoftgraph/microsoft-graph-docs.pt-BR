---
title: Relatórios de uso do site do SharePoint
description: Você pode obter uma exibição de alto nível do valor que está recebendo do SharePoint em termos do número total de arquivos que os usuários armazenam em sites SharePoint, quantos arquivos estão sendo usados ativamente e o armazenamento consumido em todos esses sites. Em seguida, você pode analisar o relatório de uso do site do SharePoint para entender as tendências e os detalhes de acordo com o nível do site para todos os sites.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: dd0f57a197981ee41b887c824eddcbcf3a2b3814
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390784"
---
# <a name="sharepoint-site-usage-reports"></a>Relatórios de uso do site do SharePoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma exibição de alto nível do valor que está recebendo do SharePoint em termos do número total de arquivos que os usuários armazenam em sites SharePoint, quantos arquivos estão sendo usados ativamente e o armazenamento consumido em todos esses sites. Em seguida, você pode analisar o relatório de uso do site do SharePoint para entender as tendências e os detalhes de acordo com o nível do site para todos os sites.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - SharePoint uso do site](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados do site](../api/reportroot-getsharepointsiteusagedetail.md) | Fluxo          | Fluxo           | Obtenha dados sobre o uso do site do SharePoint.                     |
| [Obter contagens de arquivo](../api/reportroot-getsharepointsiteusagefilecounts.md) | Fluxo          | Fluxo           | Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter contagens do site](../api/reportroot-getsharepointsiteusagesitecounts.md) | Fluxo          | Fluxo           | Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado. |
| [Obter armazenamento](../api/reportroot-getsharepointsiteusagestorage.md) | Fluxo          | Fluxo           | Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório. |
| [Obter páginas](../api/reportroot-getsharepointsiteusagepages.md) | Fluxo          | Fluxo           | Obtenha o número de páginas visualizadas em todos os sites.             |


