---
title: Relatórios de uso de dispositivos Skype for Business
description: Você pode usar os relatórios de uso do dispositivo Skype for Business para obter dados sobre os tipos de clientes e dispositivos que são usados em toda a sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: bf567349f655a3dd0a9d6c0b49affdc2892ea969
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897964"
---
# <a name="skype-for-business-device-usage-reports"></a>Relatórios de uso de dispositivos Skype for Business

Namespace: microsoft.graph

Você pode usar os relatórios de uso do dispositivo Skype for Business para obter dados sobre os tipos de clientes e dispositivos que são usados em toda a sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-clientes do Skype for Business usados](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | Stream      | Obtenha dados sobre o uso do dispositivo Skype for Business por usuário. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | Fluxo      | Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | Fluxo      | Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business. Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização. |
