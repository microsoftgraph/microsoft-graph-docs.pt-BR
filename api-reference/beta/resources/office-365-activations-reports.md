---
title: Relatórios de ativações do Office 365
description: O relatório de ativação do Office 365 fornece uma visão de quais usuários ativaram suas assinaturas do Office 365 em pelo menos um dispositivo. Ele fornece uma divisão das ativações de assinatura do Office 365 ProPlus, do Project e do Visio pro para Office 365, bem como a divisão de ativações na área de trabalho e nos dispositivos. Este relatório pode ajudá-lo a identificar os usuários que podem precisar de suporte adicional para ativar sua assinatura do Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 1e3a3831c3ea5c2b4307ae612630421365992759
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009549"
---
# <a name="office-365-activations-reports"></a>Relatórios de ativações do Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O relatório de ativação do Office 365 fornece uma visão de quais usuários ativaram suas assinaturas do Office 365 em pelo menos um dispositivo. Ele fornece uma divisão das ativações de assinatura do Office 365 ProPlus, do Project e do Visio pro para Office 365, bem como a divisão de ativações na área de trabalho e nos dispositivos. Este relatório pode ajudá-lo a identificar os usuários que podem precisar de suporte adicional para ativar sua assinatura do Office.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activationsuserdetail.md) | Fluxo          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Obtenha dados sobre usuários que ativaram o Office 365. |
| [Obter contagens de ativação](../api/reportroot-getoffice365activationcounts.md) | Fluxo          | [office365ActivationCounts](../resources/office365activationcounts.md) | Obtenha a contagem de ativações do Office 365 em desktops e dispositivos. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activationsusercounts.md) | Fluxo          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos. |
