---
title: tipo de enum vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: tfitzmac
ms.openlocfilehash: 5aa3f44f0e4ccf177154f97e9849093c52728b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343418"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>tipo de enum vpnTrafficRuleRoutingPolicyType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Especifica a política de roteamento para uma regra de tráfego VPN.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Nenhuma política de roteamento especificada.|
|splitTunnel|1|Tráfego de rede para o aplicativo especificado será roteado através da VPN.|
|forceTunnel|2|Todo o tráfego de rede será roteado através da VPN.|





