---
title: Relatórios dos usuários ativos do Office 365
description: Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças do produto estão sendo usadas por indivíduos em sua organização e fazer uma busca detalhada para obter informações sobre quais usuários estão usando quais produtos. Este relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.
localization_priority: Normal
ms.openlocfilehash: d52588630dcb18a146f34ad66c154e3a64752266
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837153"
---
# <a name="office-365-active-users-reports"></a>Relatórios dos usuários ativos do Office 365

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças do produto estão sendo usadas por indivíduos em sua organização e fazer uma busca detalhada para obter informações sobre quais usuários estão usando quais produtos. Este relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activeuserdetail.md) | Fluxo          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Obtenha dados sobre os usuários ativos do Office 365. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activeusercounts.md) | Fluxo          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | Obtenha a contagem de usuários ativos diários no período de relatório por produto. |
| [Obter contagens de usuários dos serviços](../api/reportroot-getoffice365servicesusercounts.md) | Fluxo          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | Obtenha a contagem de usuários por tipo de atividade e serviço. |
