---
title: Tipo de número vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: baf1fa3bf6edcb3358c8ae56d2572365702c41273a04bd578c2c98af5e68d0ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139597"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>Tipo de número vpnServiceExceptionAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A ação VPN a ser tomada para um serviço específico.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|forceTrafficViaVPN|0|Fazer todo o tráfego desse serviço passar pela VPN|
|allowTrafficOutside|1 |Permitir o serviço fora da VPN|
|dropTraffic|2|Soltar todo o tráfego do serviço|




