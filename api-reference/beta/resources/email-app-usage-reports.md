---
title: Relatórios de uso do aplicativo de email
description: Você pode ver quantos aplicativos de email são usados para se conectar a Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.
ms.localizationpriority: medium
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 341dda4411e39cd028f6f5921e12e1c5b5bd5d7f
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044803"
---
# <a name="email-app-usage-reports"></a>Relatórios de uso do aplicativo de email

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode ver quantos aplicativos de email são usados para se conectar a Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados de usuário](../api/reportroot-getemailappusageuserdetail.md) | Fluxo          | Fluxo           | Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email. |
| [Obter contagens de usuários do aplicativo](../api/reportroot-getemailappusageappsusercounts.md) | Fluxo          | Fluxo           | Obtenha a contagem de usuários únicos por aplicativo de email.                 |
| [Obter contagens de usuários](../api/reportroot-getemailappusageusercounts.md) | Fluxo          | Fluxo           | Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email. |
| [Obter contagens de usuários das versões](../api/reportroot-getemailappusageversionsusercounts.md) | Fluxo          | Fluxo           | Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.    |


