---
title: Relatórios de atividades do OneDrive
description: Você pode obter a atividade de todos os usuários licenciados para usar o OneDrive observando sua interação com arquivos no OneDrive. Ele também ajuda você a entender o nível de colaboração que está acontecendo mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7d0c069d2787b30f37e634757127b6141843a9ed
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983598"
---
# <a name="onedrive-activity-reports"></a>Relatórios de atividades do OneDrive

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter a atividade de cada usuário licenciado para usar o OneDrive analisando sua interação com arquivos no OneDrive. Ele também ajuda você a entender o nível de colaboração que está acontecendo mostrando o número de arquivos compartilhados.

> **Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira relatórios do [Microsoft 365 - atividade do OneDrive for Business.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getonedriveactivityuserdetail.md) | Fluxo          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | Obtenha dados sobre as atividades do OneDrive por usuário. |
| [Obter contagens de usuários](../api/reportroot-getonedriveactivityusercounts.md) | Fluxo          | [siteActivitySummary](../resources/siteactivitysummary.md) | Obtenha a tendência no número de usuários ativos do OneDrive. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveactivityfilecounts.md) | Fluxo          | [siteActivitySummary](../resources/siteactivitysummary.md) | Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive. |


