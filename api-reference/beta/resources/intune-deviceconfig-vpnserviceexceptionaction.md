---
title: tipo de enumeração vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ba0ea4081ea958d4eb36d2506c4cc4cab5ef59a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985920"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>tipo de enumeração vpnServiceExceptionAction

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A ação VPN a ser tomada para um serviço específico.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|forceTrafficViaVPN|,0|Fazer com que todo o tráfego desse serviço percorra a VPN|
|allowTrafficOutside|1 |Permitir o serviço fora da VPN|
|dropTraffic|2 |Remover todo o tráfego do serviço|






