---
title: Relatórios dos usuários ativos do Office 365
description: Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças de produtos estão sendo usadas por indivíduos em sua organização e detalhar para obter informações sobre quais usuários estão usando quais produtos. Esse relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ea93b37e4a22b733274f65d785204764afa34015
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966591"
---
# <a name="office-365-active-users-reports"></a>Relatórios dos usuários ativos do Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças de produtos estão sendo usadas por indivíduos em sua organização e detalhar para obter informações sobre quais usuários estão usando quais produtos. Esse relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activeuserdetail.md) | Fluxo          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Obtenha dados sobre os usuários ativos do Office 365. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activeusercounts.md) | Fluxo          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | Obtenha a contagem de usuários ativos diários no período de relatório por produto. |
| [Obter contagens de usuários dos serviços](../api/reportroot-getoffice365servicesusercounts.md) | Fluxo          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | Obtenha a contagem de usuários por tipo de atividade e serviço. |
