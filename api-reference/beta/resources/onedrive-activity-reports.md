---
title: Relatórios de atividades do OneDrive
description: Você pode obter a atividade de todos os usuários licenciados para usar o OneDrive examinando sua interação com os arquivos no OneDrive. Ele também ajuda a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8e02e93d2266f302fb3f90ab47fe4853e34adee5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947194"
---
# <a name="onedrive-activity-reports"></a>Relatórios de atividades do OneDrive

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode obter a atividade de todos os usuários licenciados para usar o OneDrive examinando sua interação com os arquivos no OneDrive. Ele também ajuda a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getonedriveactivityuserdetail.md) | Fluxo          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | Obtenha dados sobre as atividades do OneDrive por usuário. |
| [Obter contagens de usuários](../api/reportroot-getonedriveactivityusercounts.md) | Fluxo          | [siteActivitySummary](../resources/siteactivitysummary.md) | Obtenha a tendência no número de usuários ativos do OneDrive. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveactivityfilecounts.md) | Fluxo          | [siteActivitySummary](../resources/siteactivitysummary.md) | Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive. |
