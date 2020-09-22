---
title: Relatórios de atividades do OneDrive
description: Você pode obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Ele também ajuda você a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 656d722a9d63e460cd4b62e87a0b2fd8483e37c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092332"
---
# <a name="onedrive-activity-reports"></a>Relatórios de atividades do OneDrive

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Ele também ajuda você a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-onedrive for Business Activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getonedriveactivityuserdetail.md) | Fluxo          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | Obtenha dados sobre as atividades do OneDrive por usuário. |
| [Obter contagens de usuários](../api/reportroot-getonedriveactivityusercounts.md) | Fluxo          | [siteActivitySummary](../resources/siteactivitysummary.md) | Obtenha a tendência no número de usuários ativos do OneDrive. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveactivityfilecounts.md) | Fluxo          | [siteActivitySummary](../resources/siteactivitysummary.md) | Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive. |


