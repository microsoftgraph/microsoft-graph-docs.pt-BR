---
title: tipo de enum vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 028e49085e4a1fa5f01ac59ff00fbafd8846dfb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415002"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>tipo de enum vpnTrafficRuleRoutingPolicyType

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Especifica a política de roteamento para uma regra de tráfego VPN.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Nenhuma política de roteamento especificada.|
|splitTunnel|1|Tráfego de rede para o aplicativo especificado será roteado através da VPN.|
|forceTunnel|2|Todo o tráfego de rede será roteado através da VPN.|




