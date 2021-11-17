---
title: Relatórios de atividades do email
description: Você pode obter uma exibição de alto nível do tráfego de email em sua organização na página Relatórios. Você também pode detalhar o widget Atividade de Email para entender as tendências e detalhes por usuário da atividade de email em sua organização.
ms.localizationpriority: medium
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: d4599c3b0192289e8cd0e5c4d4aa59876aed075f
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044789"
---
# <a name="email-activity-reports"></a>Relatórios de atividades do email

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma exibição de alto nível do tráfego de email em sua organização na página Relatórios. Você também pode detalhar o widget Atividade de Email para entender as tendências e detalhes por usuário da atividade de email em sua organização.

> **Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Atividade de E-mail](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados de usuário](../api/reportroot-getemailactivityuserdetail.md) | Fluxo          | Fluxo           | Obtenha dados sobre as atividades de email que os usuários realizaram.       |
| [Obter contagens de atividade](../api/reportroot-getemailactivitycounts.md) | Fluxo          | Fluxo           | Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização. |
| [Obter contagens de usuários](../api/reportroot-getemailactivityusercounts.md) | Fluxo          | Fluxo           | Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber. |


