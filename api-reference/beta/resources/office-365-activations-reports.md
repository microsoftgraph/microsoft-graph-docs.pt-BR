---
title: Relatórios de ativações do Office 365
description: O relatório de ativação do Office 365 fornece uma visão de quais usuários ativaram suas assinaturas do Office 365 em pelo menos um dispositivo. Ele fornece uma divisão das ativações de assinatura do Office 365 proPlus, do Project e do Visio pro para Office 365, bem como a divisão de ativações na área de trabalho e nos dispositivos. Este relatório pode ajudá-lo a identificar os usuários que podem precisar de suporte adicional para ativar sua assinatura do Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581530"
---
# <a name="office-365-activations-reports"></a>Relatórios de ativações do Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O relatório de ativação do Office 365 fornece uma visão de quais usuários ativaram suas assinaturas do Office 365 em pelo menos um dispositivo. Ele fornece uma divisão das ativações de assinatura do Office 365 proPlus, do Project e do Visio pro para Office 365, bem como a divisão de ativações na área de trabalho e nos dispositivos. Este relatório pode ajudá-lo a identificar os usuários que podem precisar de suporte adicional para ativar sua assinatura do Office.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activationsuserdetail.md) | Fluxo          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Obtenha dados sobre usuários que ativaram o Office 365. |
| [Obter contagens de ativação](../api/reportroot-getoffice365activationcounts.md) | Fluxo          | [office365ActivationCounts](../resources/office365activationcounts.md) | Obtenha a contagem de ativações do Office 365 em desktops e dispositivos. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activationsusercounts.md) | Fluxo          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
