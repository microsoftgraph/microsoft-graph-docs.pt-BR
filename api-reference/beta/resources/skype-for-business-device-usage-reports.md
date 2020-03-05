---
title: Relatórios de uso de dispositivos Skype for Business
description: Você pode obter detalhes sobre os tipos de clientes e dispositivos que são usados em sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 6a006f04d710e7d7b210cb55e72a0418bdf124d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520482"
---
# <a name="skype-for-business-device-usage-reports"></a>Relatórios de uso de dispositivos Skype for Business

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre os tipos de clientes e dispositivos que são usados em sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | Stream          | [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) | Obtenha dados sobre o uso do dispositivo Skype for Business por usuário. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | Fluxo          | [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) | Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | Fluxo          | [skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md) | Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business. Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização. |
