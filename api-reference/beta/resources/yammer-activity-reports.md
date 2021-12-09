---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível de envolvimento da sua organização com o Yammer pela quantidade de atividades geradas em toda a organização e pelo número de usuários exclusivos que postam, como e leem mensagens no Yammer.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 5d157217c94d35450929745a4f5bf0989bb2bf49
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390826"
---
# <a name="yammer-activity-reports"></a>Relatórios de atividades do Yammer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode entender o nível de envolvimento da sua organização com o Yammer pela quantidade de atividades geradas em toda a organização e pelo número de usuários exclusivos que postam, como e leem mensagens no Yammer.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Yammer Atividade](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados de usuário](../api/reportroot-getyammeractivityuserdetail.md) | Fluxo          | Stream           | Obtenha dados sobre as atividades do Yammer por usuário.                   |
| [Obter contagens de atividade](../api/reportroot-getyammeractivitycounts.md) | Fluxo          | Stream           | Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas. |
| [Obter contagens de usuários](../api/reportroot-getyammeractivityusercounts.md) | Fluxo          | Stream           | Obter as tendências sobre o número de usuários exclusivos que postaram, leram e gostaram Yammer mensagens. |


