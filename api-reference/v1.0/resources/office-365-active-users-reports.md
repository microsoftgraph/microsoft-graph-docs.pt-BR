---
title: Relatórios dos usuários ativos do Office 365
description: Você pode usar os relatórios dos usuários ativos do Office 365 para descobrir quantas licenças de produtos estão sendo usadas por indivíduos em sua organização e detalhar informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 163eab83bfcb5089ec21d449d90840384c12e4ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447343"
---
# <a name="office-365-active-users-reports"></a>Relatórios dos usuários ativos do Office 365

Namespace: Microsoft. Graph

Você pode usar os relatórios dos usuários ativos do Office 365 para descobrir quantas licenças de produtos estão sendo usadas por indivíduos em sua organização e detalhar informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activeuserdetail.md) | Stream      | Obtenha dados sobre os usuários ativos do Office 365. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activeusercounts.md) | Fluxo      | Obtenha a contagem de usuários ativos diários no período de relatório por produto. |
| [Obter contagens de usuários dos serviços](../api/reportroot-getoffice365servicesusercounts.md) | Fluxo      | Obtenha a contagem de usuários por tipo de atividade e serviço. |
