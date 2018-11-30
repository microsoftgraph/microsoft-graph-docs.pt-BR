---
title: Relatórios de atividades do OneDrive
description: Você pode obter a atividade de todos os usuários licenciados para usar o OneDrive examinando sua interação com os arquivos no OneDrive. Ele também ajuda a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.
ms.openlocfilehash: cfcae36cad301c777eea4ede4532efda0ce13b39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040796"
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
