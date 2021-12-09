---
title: Yammer de uso do dispositivo
description: Os relatórios de uso do dispositivo Yammer informações sobre quais dispositivos seus usuários utilizam para se envolver Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b9d5a7d2ea6cd8e02e26414618b27acf441444cd
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390050"
---
# <a name="yammer-device-usage-reports"></a>Yammer de uso do dispositivo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os relatórios de uso do dispositivo Yammer informações sobre quais dispositivos seus usuários utilizam para se envolver Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Yammer uso do dispositivo](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                    |
| :----------------------------------------------------------- | :-------------- | :--------------- | ---------------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammerdeviceusageuserdetail.md) | Fluxo          | Stream           | Obtenha dados sobre o uso do dispositivo Yammer por usuário. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Fluxo          | Stream           | Obtenha o número de usuários por tipo de dispositivo.        |
| [Obter contagens de usuários](../api/reportroot-getyammerdeviceusageusercounts.md) | Fluxo          | Stream           | Obtenha o número de usuários diários por tipo de dispositivo.  |


