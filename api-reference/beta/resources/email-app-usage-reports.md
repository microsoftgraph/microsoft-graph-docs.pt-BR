---
title: Relatórios de uso do aplicativo de email
description: Você pode ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: df40e61108a3933801f5e7c21057f71600b496ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340186"
---
# <a name="email-app-usage-reports"></a>Relatórios de uso do aplicativo de email

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getemailappusageuserdetail.md) | Fluxo          | [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) | Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email. |
| [Obter contagens de usuários do aplicativo](../api/reportroot-getemailappusageappsusercounts.md) | Fluxo          | [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) | Obtenha a contagem de usuários únicos por aplicativo de email. |
| [Obter contagens de usuários](../api/reportroot-getemailappusageusercounts.md) | Fluxo          | [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) | Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email. |
| [Obter contagens de usuários das versões](../api/reportroot-getemailappusageversionsusercounts.md) | Fluxo          | [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) | Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook. |
