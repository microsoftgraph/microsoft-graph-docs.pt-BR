---
title: Relatórios de atividades do OneDrive
description: Use os relatórios de atividades do OneDrive para obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Esses relatórios podem ajudar você a entender o nível de colaboração acontecendo, mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 24a2e74e9e117c13fa49efc6fba4323f75716ffe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898146"
---
# <a name="onedrive-activity-reports"></a>Relatórios de atividades do OneDrive

Namespace: microsoft.graph

Use os relatórios de atividades do OneDrive para obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Esses relatórios podem ajudar você a entender o nível de colaboração acontecendo, mostrando o número de arquivos compartilhados.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-onedrive for Business Activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getonedriveactivityuserdetail.md) | Stream      | Obtenha dados sobre as atividades do OneDrive por usuário. |
| [Obter contagens de usuários](../api/reportroot-getonedriveactivityusercounts.md) | Fluxo      | Obtenha a tendência no número de usuários ativos do OneDrive. |
| [Obter contagens de arquivo](../api/reportroot-getonedriveactivityfilecounts.md) | Fluxo      | Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive. |

