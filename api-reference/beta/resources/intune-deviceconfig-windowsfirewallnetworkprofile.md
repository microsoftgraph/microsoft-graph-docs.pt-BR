---
title: Tipo de recurso windowsFirewallNetworkProfile
description: Políticas de perfil do firewall do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1b17382277e5bad323bbaf54ca191b6ae22b6935c9d921f8ca86bc172f44d65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54173097"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Tipo de recurso windowsFirewallNetworkProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Políticas de perfil do firewall do Windows.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Configura o dispositivo host para permitir ou bloquear o firewall e a imposição de segurança avançada para o perfil de rede. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|stealthModeRequired|Boolean|Permitir que o servidor opere no modo de discrição. Quando o StealthModeRequired e o StealthModeBlocked são verdadeiros, o StealthModeBlocked tem prioridade.|
|stealthModeBlocked|Booliano|Impedir que o servidor operando no modo de furtividade. Quando o StealthModeRequired e o StealthModeBlocked são verdadeiros, o StealthModeBlocked tem prioridade.|
|incomingTrafficRequired|Boolean|Configura o firewall para permitir o tráfego de entrada de acordo com outras configurações de política. Quando IncomingTrafficRequired e IncomingTrafficBlocked são verdadeiros, IncomingTrafficBlocked tem prioridade.|
|incomingTrafficBlocked|Booliano|Configura o firewall para bloquear todo o tráfego de entrada, independentemente de outras configurações de política. Quando IncomingTrafficRequired e IncomingTrafficBlocked são verdadeiros, IncomingTrafficBlocked tem prioridade.|
|unicastResponsesToMulticastBroadcastsRequired|Boolean|Configura o firewall para permitir respostas unicast ao tráfego de transmissão multicast. Quando UnicastResponsesToMulticastBroadcastsRequired e UnicastResponsesToMulticastBroadcastsBlocked são verdadeiros, UnicastResponsesToMulticastBroadcastsBlocked tem prioridade.|
|unicastResponsesToMulticastBroadcastsBlocked|Booliano|Configura o firewall para bloquear respostas unicast ao tráfego de transmissão multicast. Quando UnicastResponsesToMulticastBroadcastsRequired e UnicastResponsesToMulticastBroadcastsBlocked são verdadeiros, UnicastResponsesToMulticastBroadcastsBlocked tem prioridade.|
|inboundNotificationsRequired|Boolean|Permite que o firewall exibe notificações quando um aplicativo é impedido de ouvir em uma porta. Quando InboundNotificationsRequired e InboundNotificationsBlocked são verdadeiros, InboundNotificationsBlocked tem prioridade.|
|inboundNotificationsBlocked|Booliano|Impede que o firewall exibe notificações quando um aplicativo é bloqueado para ouvir em uma porta. Quando InboundNotificationsRequired e InboundNotificationsBlocked são verdadeiros, InboundNotificationsBlocked tem prioridade.|
|authorizedApplicationRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar regras de aplicativo autorizado da política de grupo com aquelas do armazenamento local em vez de ignorar as regras do armazenamento local. Quando AuthorizedApplicationRulesFromGroupPolicyNotMerged e AuthorizedApplicationRulesFromGroupPolicyMerged são verdadeiros, AuthorizedApplicationRulesFromGroupPolicyMerged tem prioridade.|
|authorizedApplicationRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclação de regras de aplicativo autorizado da política de grupo com aquelas do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando AuthorizedApplicationRulesFromGroupPolicyNotMerged e AuthorizedApplicationRulesFromGroupPolicyMerged são verdadeiros, AuthorizedApplicationRulesFromGroupPolicyMerged tem prioridade.|
|globalPortRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar regras de porta globais da política de grupo com aquelas do armazenamento local em vez de ignorar as regras de armazenamento local. Quando GlobalPortRulesFromGroupPolicyNotMerged e GlobalPortRulesFromGroupPolicyMerged são verdadeiros, GlobalPortRulesFromGroupPolicyMerged tem prioridade.|
|globalPortRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclação de regras de porta globais da política de grupo com aquelas do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando GlobalPortRulesFromGroupPolicyNotMerged e GlobalPortRulesFromGroupPolicyMerged são verdadeiros, GlobalPortRulesFromGroupPolicyMerged tem prioridade.|
|connectionSecurityRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar regras de segurança de conexão da política de grupo com aquelas do armazenamento local em vez de ignorar as regras do armazenamento local. Quando ConnectionSecurityRulesFromGroupPolicyNotMerged e ConnectionSecurityRulesFromGroupPolicyMerged são verdadeiros, ConnectionSecurityRulesFromGroupPolicyMerged tem prioridade.|
|connectionSecurityRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclação de regras de segurança de conexão da política de grupo com aquelas do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando ConnectionSecurityRulesFromGroupPolicyNotMerged e ConnectionSecurityRulesFromGroupPolicyMerged são verdadeiros, ConnectionSecurityRulesFromGroupPolicyMerged tem prioridade.|
|outboundConnectionsRequired|Boolean|Configura o firewall para permitir todas as conexões de saída por padrão. Quando OutboundConnectionsRequired e OutboundConnectionsBlocked são verdadeiros, OutboundConnectionsBlocked tem prioridade. Essa configuração será aplicada ao Windows versão 1809 e superior.|
|outboundConnectionsBlocked|Booliano|Configura o firewall para bloquear todas as conexões de saída por padrão. Quando OutboundConnectionsRequired e OutboundConnectionsBlocked são verdadeiros, OutboundConnectionsBlocked tem prioridade. Essa configuração será aplicada ao Windows versão 1809 e superior.|
|inboundConnectionsRequired|Boolean|Configura o firewall para permitir todas as conexões de entrada por padrão. Quando InboundConnectionsRequired e InboundConnectionsBlocked são verdadeiros, InboundConnectionsBlocked tem prioridade.|
|inboundConnectionsBlocked|Booliano|Configura o firewall para bloquear todas as conexões de entrada por padrão. Quando InboundConnectionsRequired e InboundConnectionsBlocked são verdadeiros, InboundConnectionsBlocked tem prioridade.|
|securedPacketExemptionAllowed|Booliano|Configura o firewall para permitir que o computador host responda ao tráfego de rede não solicitado desse tráfego é protegido pelo IPSec mesmo quando o stealthModeBlocked é definido como true. Quando SecuredPacketExemptionBlocked e SecuredPacketExemptionAllowed são verdadeiros, SecuredPacketExemptionAllowed tem prioridade.|
|securedPacketExemptionBlocked|Boolean|Configura o firewall para bloquear o computador host para responder ao tráfego de rede não solicitado desse tráfego é protegido pelo IPSec mesmo quando o stealthModeBlocked é definido como true. Quando SecuredPacketExemptionBlocked e SecuredPacketExemptionAllowed são verdadeiros, SecuredPacketExemptionAllowed tem prioridade.|
|policyRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar políticas de Regra de Firewall da política de grupo com aquelas do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando PolicyRulesFromGroupPolicyNotMerged e PolicyRulesFromGroupPolicyMerged são verdadeiros, PolicyRulesFromGroupPolicyMerged tem prioridade.|
|policyRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclação de políticas de Regra de Firewall da política de grupo com aquelas do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando PolicyRulesFromGroupPolicyNotMerged e PolicyRulesFromGroupPolicyMerged são verdadeiros, PolicyRulesFromGroupPolicyMerged tem prioridade.|

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




