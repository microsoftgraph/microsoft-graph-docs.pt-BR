---
title: Relatórios de usuários ativos do Microsoft 365
description: Você pode usar os relatórios do Microsoft 365 active Users para saber quantas licenças de produto estão sendo usadas por indivíduos em sua organização e detalhar as informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 041bbe180df2225383d704002d06359334fb8d84
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898160"
---
# <a name="microsoft-365-active-users-reports"></a>Relatórios de usuários ativos do Microsoft 365

Namespace: microsoft.graph

Você pode usar os relatórios do Microsoft 365 active Users para saber quantas licenças de produto estão sendo usadas por indivíduos em sua organização e detalhar as informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activeuserdetail.md) | Stream      | Obtenha detalhes sobre usuários ativos do Microsoft 365. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activeusercounts.md) | Fluxo      | Obtenha a contagem de usuários ativos diários no período de relatório por produto. |
| [Obter contagens de usuários dos serviços](../api/reportroot-getoffice365servicesusercounts.md) | Fluxo      | Obtenha a contagem de usuários por tipo de atividade e serviço. |
