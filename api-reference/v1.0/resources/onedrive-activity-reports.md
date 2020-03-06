---
title: Relatórios de atividades do OneDrive
description: Use os relatórios de atividades do OneDrive para obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Esses relatórios podem ajudar você a entender o nível de colaboração acontecendo, mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0399b7e3d320efbc98c3cf25cd2830a4749d8df5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534167"
---
# <a name="onedrive-activity-reports"></a>Relatórios de atividades do OneDrive

Namespace: microsoft.graph

Use os relatórios de atividades do OneDrive para obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Esses relatórios podem ajudar você a entender o nível de colaboração acontecendo, mostrando o número de arquivos compartilhados.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getonedriveactivityuserdetail.md) | Stream      | Obtenha dados sobre as atividades do OneDrive por usuário. |
| [Obter contagens de usuários](../api/reportroot-getonedriveactivityusercounts.md) | Fluxo      | Obtenha a tendência no número de usuários ativos do OneDrive. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveactivityfilecounts.md) | Fluxo      | Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive. |

