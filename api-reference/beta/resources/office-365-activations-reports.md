---
title: Relatórios de ativações do Microsoft 365
description: O relatório de ativação do Microsoft 365 oferece uma visão de quais usuários ativaram suas assinaturas do Microsoft 365 em pelo menos um dispositivo. Ele fornece uma divisão das ativações de assinatura do Microsoft 365 ProPlus, Project e Visio Pro para Microsoft 365, bem como o detalhamento das ativações em computadores e dispositivos. Esse relatório pode ajudá-lo a identificar usuários que podem precisar de suporte adicional para ativar a assinatura do Office.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 32fb2f1397218a5d6c99b071b7a398cf00cd54f7
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980789"
---
# <a name="microsoft-365-activations-reports"></a>Relatórios de ativações do Microsoft 365

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O relatório de ativação do Microsoft 365 oferece uma visão de quais usuários ativaram suas assinaturas do Microsoft 365 em pelo menos um dispositivo. Ele fornece uma divisão das ativações de assinatura do Microsoft 365 ProPlus, Project e Visio Pro para Microsoft 365, bem como o detalhamento das ativações em computadores e dispositivos. Esse relatório pode ajudá-lo a identificar usuários que podem precisar de suporte adicional para ativar a assinatura do Office.

> **Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - ativações do Microsoft Office.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activationsuserdetail.md) | Fluxo          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Obter detalhes sobre os usuários que ativaram o Microsoft 365. |
| [Obter contagens de ativação](../api/reportroot-getoffice365activationcounts.md) | Fluxo          | [office365ActivationCounts](../resources/office365activationcounts.md) | Obter a contagem de ativações do Microsoft 365 em desktops e dispositivos. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activationsusercounts.md) | Fluxo          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos. |


