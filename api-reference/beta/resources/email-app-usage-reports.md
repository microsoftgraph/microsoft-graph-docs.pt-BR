---
title: Relatórios de uso do aplicativo de email
description: Você pode ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: f666fed390272002f2e556f355618fddc935981e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896900"
---
# <a name="email-app-usage-reports"></a>Relatórios de uso do aplicativo de email

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getemailappusageuserdetail.md) | Stream          | [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) | Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email. |
| [Obter contagens de usuários do aplicativo](../api/reportroot-getemailappusageappsusercounts.md) | Stream          | [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) | Obtenha a contagem de usuários únicos por aplicativo de email. |
| [Obter contagens de usuários](../api/reportroot-getemailappusageusercounts.md) | Fluxo          | [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) | Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email. |
| [Obter contagens de usuários das versões](../api/reportroot-getemailappusageversionsusercounts.md) | Fluxo          | [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) | Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook. |
