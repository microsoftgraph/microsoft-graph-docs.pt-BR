---
title: Tipo de número vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: be93dbef587a897d10d13b54bddbd738418b12bf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026963"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>Tipo de número vpnTrafficRuleRoutingPolicyType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especifica a política de roteamento para uma regra de tráfego VPN.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Nenhuma política de roteamento especificada.|
|splitTunnel|1|O tráfego de rede para o aplicativo especificado será roteado pela VPN.|
|forceTunnel|2|Todo o tráfego de rede será roteado pela VPN.|



