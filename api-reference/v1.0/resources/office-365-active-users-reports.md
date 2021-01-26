---
title: Relatórios de usuários ativos do Microsoft 365
description: Você pode usar os relatórios de usuários ativos do Microsoft 365 para descobrir quantas licenças de produto estão sendo usadas por indivíduos em sua organização e fazer buscas drill down para obter informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e795b58eaae7ecd428f1473b277cd6bc65cbf09d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981022"
---
# <a name="microsoft-365-active-users-reports"></a>Relatórios de usuários ativos do Microsoft 365

Namespace: microsoft.graph

Você pode usar os relatórios de usuários ativos do Microsoft 365 para descobrir quantas licenças de produto estão sendo usadas por indivíduos em sua organização e fazer buscas drill down para obter informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.

> **Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Usuários Ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d). 

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activeuserdetail.md) | Fluxo      | Obter detalhes sobre usuários ativos do Microsoft 365. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activeusercounts.md) | Fluxo      | Obtenha a contagem de usuários ativos diários no período de relatório por produto. |
| [Obter contagens de usuários dos serviços](../api/reportroot-getoffice365servicesusercounts.md) | Fluxo      | Obtenha a contagem de usuários por tipo de atividade e serviço. |

