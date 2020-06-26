---
title: Relatórios de ativações do Microsoft 365
description: Os relatórios de ativação do Microsoft 365 podem fornecer uma visão de quais usuários ativaram suas assinaturas do Microsoft 365 em pelo menos um dispositivo. Esses relatórios fornecem uma divisão das ativações de assinatura do Microsoft 365 ProPlus, do Project e do Visio pro para Office 365, bem como a divisão de ativações na área de trabalho e nos dispositivos. Esses relatórios podem ajudar a identificar os usuários que podem precisar de suporte adicional para ativar a assinatura do Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 34bebb8edb7d83ca631d93add90a7e2810849c3d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898167"
---
# <a name="microsoft-365-activations-reports"></a>Relatórios de ativações do Microsoft 365

Namespace: microsoft.graph

Os relatórios de ativação do Microsoft 365 podem fornecer uma visão de quais usuários ativaram suas assinaturas do Microsoft 365 em pelo menos um dispositivo. Esses relatórios fornecem uma divisão das ativações de assinatura do Microsoft 365 ProPlus, do Project e do Visio pro para Office 365, bem como a divisão de ativações na área de trabalho e nos dispositivos. Esses relatórios podem ajudar a identificar os usuários que podem precisar de suporte adicional para ativar a assinatura do Office.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activationsuserdetail.md) | Stream      | Obtenha detalhes sobre os usuários que ativaram o Microsoft 365. |
| [Obter contagens de ativação](../api/reportroot-getoffice365activationcounts.md) | Fluxo      | Obtenha a contagem de ativações do Microsoft 365 em desktops e dispositivos. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activationsusercounts.md) | Fluxo      | Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos. |
