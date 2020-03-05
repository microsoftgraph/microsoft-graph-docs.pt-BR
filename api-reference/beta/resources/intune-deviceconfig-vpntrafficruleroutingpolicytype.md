---
title: tipo de enumeração vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d26e9c84f21fb952d4db58ef5faf28d1b696454
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529269"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>tipo de enumeração vpnTrafficRuleRoutingPolicyType

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especifica a política de roteamento para uma regra de tráfego VPN.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhuma|,0|Nenhuma política de roteamento especificada.|
|splitTunnel|1 |O tráfego de rede do aplicativo especificado será roteado através da VPN.|
|forceTunnel|2 |Todo o tráfego de rede será roteado através da VPN.|



