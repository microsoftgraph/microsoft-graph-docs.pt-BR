---
title: Relatórios de usuários ativos do Microsoft 365
description: Você pode usar o relatório do Microsoft 365 active Users para saber quantas licenças de produto estão sendo usadas por indivíduos em sua organização e detalhar as informações sobre quais usuários estão usando quais produtos. Esse relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 3d795c3308b7c1494bbff2a24545ba4ca8053583
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021242"
---
# <a name="microsoft-365-active-users-reports"></a>Relatórios de usuários ativos do Microsoft 365

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o relatório do Microsoft 365 active Users para saber quantas licenças de produto estão sendo usadas por indivíduos em sua organização e detalhar as informações sobre quais usuários estão usando quais produtos. Esse relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activeuserdetail.md) | Fluxo          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Obtenha detalhes sobre usuários ativos do Microsoft 365. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activeusercounts.md) | Fluxo          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | Obtenha a contagem de usuários ativos diários no período de relatório por produto. |
| [Obter contagens de usuários dos serviços](../api/reportroot-getoffice365servicesusercounts.md) | Fluxo          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | Obtenha a contagem de usuários por tipo de atividade e serviço. |


