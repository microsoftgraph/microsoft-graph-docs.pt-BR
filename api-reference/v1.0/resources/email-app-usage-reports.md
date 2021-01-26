---
title: Relatórios de uso do aplicativo de email
description: Use os relatórios de uso do aplicativo de email para ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: df0b0bcea7631551ff0dc75162b9d294a7760f99
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981668"
---
# <a name="email-app-usage-reports"></a>Relatórios de uso do aplicativo de email

Namespace: microsoft.graph

Use os relatórios de uso do aplicativo de email para ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.

> **Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - Uso de aplicativos de email.](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getemailappusageuserdetail.md) | Fluxo      | Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email. |
| [Obter contagens de usuários do aplicativo](../api/reportroot-getemailappusageappsusercounts.md) | Fluxo      | Obtenha a contagem de usuários únicos por aplicativo de email. |
| [Obter contagens de usuários](../api/reportroot-getemailappusageusercounts.md) | Fluxo      | Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email. |
| [Obter contagens de usuários das versões](../api/reportroot-getemailappusageversionsusercounts.md) | Fluxo      | Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook. |

