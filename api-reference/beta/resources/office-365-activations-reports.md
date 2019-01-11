---
title: Relatórios de ativações do Office 365
description: O relatório de ativação do Office 365 oferece um modo de exibição dos quais usuários ativou suas assinaturas do Office 365 em pelo menos um dispositivo. Ele fornece uma divisão do Office 365 ProPlus, Project e Visio Pro para Office 365 ativações de assinatura, bem como a divisão da ativações entre dispositivos e área de trabalho. Este relatório pode ajudá-lo a identificar os usuários que talvez seja necessário suporte adicional para ativar sua assinatura do Office.
localization_priority: Normal
ms.openlocfilehash: 2576579879e60573a9ed70f805fe07532bab8ad8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822215"
---
# <a name="office-365-activations-reports"></a>Relatórios de ativações do Office 365

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O relatório de ativação do Office 365 oferece um modo de exibição dos quais usuários ativou suas assinaturas do Office 365 em pelo menos um dispositivo. Ele fornece uma divisão do Office 365 ProPlus, Project e Visio Pro para Office 365 ativações de assinatura, bem como a divisão da ativações entre dispositivos e área de trabalho. Este relatório pode ajudá-lo a identificar os usuários que talvez seja necessário suporte adicional para ativar sua assinatura do Office.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activationsuserdetail.md) | Fluxo          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Obtenha dados sobre usuários que ativaram o Office 365. |
| [Obter contagens de ativação](../api/reportroot-getoffice365activationcounts.md) | Fluxo          | [office365ActivationCounts](../resources/office365activationcounts.md) | Obtenha a contagem de ativações do Office 365 em desktops e dispositivos. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activationsusercounts.md) | Fluxo          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos. |
