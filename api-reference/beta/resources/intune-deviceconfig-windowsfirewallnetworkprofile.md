---
title: Tipo de recurso windowsFirewallNetworkProfile
description: Políticas de perfil do firewall do Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 187fd992231178300d98273f83e4310857a38261
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419720"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Tipo de recurso windowsFirewallNetworkProfile

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Políticas de perfil do firewall do Windows.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Configura o dispositivo de host para permitir ou bloquear o firewall e imposição de segurança avançada para o perfil de rede. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|stealthModeRequired|Boolean|Permitir que o servidor operar no modo oculto. Quando StealthModeRequired e StealthModeBlocked são ambos true, StealthModeBlocked tem prioridade.|
|stealthModeBlocked|Booliano|Impedir que o servidor operando em modo oculto. Quando StealthModeRequired e StealthModeBlocked são ambos true, StealthModeBlocked tem prioridade.|
|incomingTrafficRequired|Boolean|Configura o firewall para permitir o tráfego de entrada de acordo com a outras configurações de diretiva. Quando IncomingTrafficRequired e IncomingTrafficBlocked são ambos true, IncomingTrafficBlocked tem prioridade.|
|incomingTrafficBlocked|Booliano|Configura o firewall para bloquear todo o tráfego de entrada independentemente das outras configurações de política. Quando IncomingTrafficRequired e IncomingTrafficBlocked são ambos true, IncomingTrafficBlocked tem prioridade.|
|unicastResponsesToMulticastBroadcastsRequired|Boolean|Configura o firewall para permitir respostas unicast para tráfego de transmissão multicast. Quando UnicastResponsesToMulticastBroadcastsRequired e UnicastResponsesToMulticastBroadcastsBlocked são ambos true, UnicastResponsesToMulticastBroadcastsBlocked tem prioridade.|
|unicastResponsesToMulticastBroadcastsBlocked|Booliano|Configura o firewall para bloquear respostas de unicast para tráfego de transmissão multicast. Quando UnicastResponsesToMulticastBroadcastsRequired e UnicastResponsesToMulticastBroadcastsBlocked são ambos true, UnicastResponsesToMulticastBroadcastsBlocked tem prioridade.|
|inboundNotificationsRequired|Boolean|Permite que o firewall exibir notificações quando um aplicativo é impedido de escutando em uma porta. Quando InboundNotificationsRequired e InboundNotificationsBlocked são ambos true, InboundNotificationsBlocked tem prioridade.|
|inboundNotificationsBlocked|Booliano|Impede que o firewall exiba notificações quando um aplicativo é impedido de escutando em uma porta. Quando InboundNotificationsRequired e InboundNotificationsBlocked são ambos true, InboundNotificationsBlocked tem prioridade.|
|authorizedApplicationRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar as regras de aplicativo autorizado da política de grupo com as de armazenamento local, em vez de ignorando as regras de armazenamento local. Quando AuthorizedApplicationRulesFromGroupPolicyNotMerged e AuthorizedApplicationRulesFromGroupPolicyMerged são ambos true, AuthorizedApplicationRulesFromGroupPolicyMerged tem prioridade.|
|authorizedApplicationRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclagem aplicativo autorizado regras da política de grupo com aqueles do repositório local, em vez de ignorando o local de armazenam regras. Quando AuthorizedApplicationRulesFromGroupPolicyNotMerged e AuthorizedApplicationRulesFromGroupPolicyMerged são ambos true, AuthorizedApplicationRulesFromGroupPolicyMerged tem prioridade.|
|globalPortRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar as regras de porta global da política de grupo com as de armazenamento local, em vez de ignorando as regras de armazenamento local. Quando GlobalPortRulesFromGroupPolicyNotMerged e GlobalPortRulesFromGroupPolicyMerged são ambos true, GlobalPortRulesFromGroupPolicyMerged tem prioridade.|
|globalPortRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclagem de regras de porta global da política de grupo com as de armazenamento local, em vez de ignorando as regras de armazenamento local. Quando GlobalPortRulesFromGroupPolicyNotMerged e GlobalPortRulesFromGroupPolicyMerged são ambos true, GlobalPortRulesFromGroupPolicyMerged tem prioridade.|
|connectionSecurityRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar as regras de segurança de conexão da política de grupo com as de armazenamento local, em vez de ignorando as regras de armazenamento local. Quando ConnectionSecurityRulesFromGroupPolicyNotMerged e ConnectionSecurityRulesFromGroupPolicyMerged são ambos true, ConnectionSecurityRulesFromGroupPolicyMerged tem prioridade.|
|connectionSecurityRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclagem de regras de segurança de conexão da política de grupo com aqueles do repositório local, em vez de ignorando o local de armazenam regras. Quando ConnectionSecurityRulesFromGroupPolicyNotMerged e ConnectionSecurityRulesFromGroupPolicyMerged são ambos true, ConnectionSecurityRulesFromGroupPolicyMerged tem prioridade.|
|outboundConnectionsRequired|Boolean|Configura o firewall para permitir todas as conexões de saída por padrão. Quando OutboundConnectionsRequired e OutboundConnectionsBlocked são ambos true, OutboundConnectionsBlocked tem prioridade.|
|outboundConnectionsBlocked|Booliano|Configura o firewall para bloquear todas as conexões de saída por padrão. Quando OutboundConnectionsRequired e OutboundConnectionsBlocked são ambos true, OutboundConnectionsBlocked tem prioridade.|
|inboundConnectionsRequired|Boolean|Configura o firewall para permitir todas as conexões de entrada por padrão. Quando InboundConnectionsRequired e InboundConnectionsBlocked são ambos true, InboundConnectionsBlocked tem prioridade.|
|inboundConnectionsBlocked|Booliano|Configura o firewall para bloquear todas as conexões de entrada por padrão. Quando InboundConnectionsRequired e InboundConnectionsBlocked são ambos true, InboundConnectionsBlocked tem prioridade.|
|securedPacketExemptionAllowed|Booliano|Configura o firewall para permitir que o computador host responder ao tráfego de rede não solicitadas de que o tráfego é protegido pelo IPSec mesmo quando stealthModeBlocked está definida como true. Quando SecuredPacketExemptionBlocked e SecuredPacketExemptionAllowed são ambos true, SecuredPacketExemptionAllowed tem prioridade.|
|securedPacketExemptionBlocked|Boolean|Configura o firewall para bloquear o computador host para responder ao tráfego de rede não solicitadas de que o tráfego é protegido pelo IPSec mesmo quando stealthModeBlocked está definida como true. Quando SecuredPacketExemptionBlocked e SecuredPacketExemptionAllowed são ambos true, SecuredPacketExemptionAllowed tem prioridade.|
|policyRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar as políticas de regra de Firewall da política de grupo com as de armazenamento local, em vez de ignorando as regras de armazenamento local. Quando PolicyRulesFromGroupPolicyNotMerged e PolicyRulesFromGroupPolicyMerged são ambos true, PolicyRulesFromGroupPolicyMerged tem prioridade.|
|policyRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclagem de regra de Firewall políticas da política de grupo com aqueles do repositório local, em vez de ignorando o local de armazenam regras. Quando PolicyRulesFromGroupPolicyNotMerged e PolicyRulesFromGroupPolicyMerged são ambos true, PolicyRulesFromGroupPolicyMerged tem prioridade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeRequired": true,
  "stealthModeBlocked": true,
  "incomingTrafficRequired": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsRequired": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsRequired": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyNotMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyNotMerged": true,
  "outboundConnectionsRequired": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsRequired": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "securedPacketExemptionBlocked": true,
  "policyRulesFromGroupPolicyMerged": true,
  "policyRulesFromGroupPolicyNotMerged": true
}
```




