---
title: Microsoft 365 relatórios de ativações
description: O Microsoft 365 de ativação oferece uma exibição de quais usuários ativaram suas assinaturas Microsoft 365 em pelo menos um dispositivo. Ele fornece uma divisão do Microsoft 365 ProPlus, Project e Visio Pro para ativações de assinatura do Microsoft 365, bem como a divisão de ativações entre a área de trabalho e dispositivos. Este relatório pode ajudá-lo a identificar usuários que podem precisar de suporte adicional para ativar a assinatura Office assinatura.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: ca3a0218b288105982cb67664629a467a67d596a
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390624"
---
# <a name="microsoft-365-activations-reports"></a>Microsoft 365 relatórios de ativações

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft 365 de ativação oferece uma exibição de quais usuários ativaram suas assinaturas Microsoft 365 em pelo menos um dispositivo. Ele fornece uma divisão do Microsoft 365 ProPlus, Project e Visio Pro para ativações de assinatura do Microsoft 365, bem como a divisão de ativações entre a área de trabalho e dispositivos. Este relatório pode ajudá-lo a identificar usuários que podem precisar de suporte adicional para ativar a assinatura Office assinatura.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Microsoft Office ativações](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Relatórios
| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados de usuário](../api/reportroot-getoffice365activationsuserdetail.md) | Fluxo          | Stream           | Obter detalhes sobre usuários que ativaram Microsoft 365.    |
| [Obter contagens de ativação](../api/reportroot-getoffice365activationcounts.md) | Fluxo          | Stream           | Obter a contagem de Microsoft 365 ativações em desktops e dispositivos. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activationsusercounts.md) | Fluxo          | Fluxo           | Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos. |


