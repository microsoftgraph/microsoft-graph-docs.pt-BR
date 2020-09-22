---
title: Relatórios de ativações do Microsoft 365
description: O relatório de ativação do Microsoft 365 fornece uma visão de quais usuários ativaram suas assinaturas do Microsoft 365 em pelo menos um dispositivo. Ele fornece uma divisão das ativações de assinatura do Microsoft 365 ProPlus, do Project e do Visio pro para Microsoft 365, bem como a divisão de ativações na área de trabalho e nos dispositivos. Este relatório pode ajudá-lo a identificar os usuários que podem precisar de suporte adicional para ativar sua assinatura do Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 86a418e75fee70d16009f0ab6f8a3f0f474760cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021256"
---
# <a name="microsoft-365-activations-reports"></a>Relatórios de ativações do Microsoft 365

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O relatório de ativação do Microsoft 365 fornece uma visão de quais usuários ativaram suas assinaturas do Microsoft 365 em pelo menos um dispositivo. Ele fornece uma divisão das ativações de assinatura do Microsoft 365 ProPlus, do Project e do Visio pro para Microsoft 365, bem como a divisão de ativações na área de trabalho e nos dispositivos. Este relatório pode ajudá-lo a identificar os usuários que podem precisar de suporte adicional para ativar sua assinatura do Office.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activationsuserdetail.md) | Fluxo          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Obtenha detalhes sobre os usuários que ativaram o Microsoft 365. |
| [Obter contagens de ativação](../api/reportroot-getoffice365activationcounts.md) | Fluxo          | [office365ActivationCounts](../resources/office365activationcounts.md) | Obtenha a contagem de ativações do Microsoft 365 em desktops e dispositivos. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activationsusercounts.md) | Fluxo          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos. |


