---
title: Relatórios de atividades do OneDrive
description: Você pode obter a atividade de cada usuário licenciado para usar OneDrive observando sua interação com arquivos em OneDrive. Ele também ajuda você a entender o nível de colaboração que está acontecendo mostrando o número de arquivos compartilhados.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 188cb9ff8fc6750a1beb4177a82e3c1135da20bb
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390791"
---
# <a name="onedrive-activity-reports"></a>Relatórios de atividades do OneDrive

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter a atividade de cada usuário licenciado para usar OneDrive observando sua interação com arquivos em OneDrive. Ele também ajuda você a entender o nível de colaboração que está acontecendo mostrando o número de arquivos compartilhados.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - OneDrive for Business atividade](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados de usuário](../api/reportroot-getonedriveactivityuserdetail.md) | Fluxo          | Fluxo           | Obtenha dados sobre as atividades do OneDrive por usuário.                 |
| [Obter contagens de usuários](../api/reportroot-getonedriveactivityusercounts.md) | Fluxo          | Fluxo           | Obtenha a tendência no número de usuários ativos do OneDrive.        |
| [Obter contagens de arquivo](../api/reportroot-getonedriveactivityfilecounts.md) | Fluxo          | Fluxo           | Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive. |


