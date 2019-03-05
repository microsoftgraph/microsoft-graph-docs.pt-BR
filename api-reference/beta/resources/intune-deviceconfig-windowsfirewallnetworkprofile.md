---
title: Tipo de recurso windowsFirewallNetworkProfile
description: Políticas de perfil do firewall do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae504c8224be18766da49108a3b80c5aecb48b71
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149774"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Tipo de recurso windowsFirewallNetworkProfile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Políticas de perfil do firewall do Windows.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Configura o dispositivo host para permitir ou bloquear o firewall e a imposição de segurança avançada para o perfil de rede. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|stealthModeRequired|Boolean|Permitir que o servidor opere em modo oculto. Quando StealthModeRequired e StealthModeBlocked são true, StealthModeBlocked tem prioridade.|
|stealthModeBlocked|Boolean|Impedir que o servidor opere em modo oculto. Quando StealthModeRequired e StealthModeBlocked são true, StealthModeBlocked tem prioridade.|
|incomingTrafficRequired|Boolean|Configura o firewall para permitir o tráfego de entrada de acordo com outras configurações de política. Quando IncomingTrafficRequired e IncomingTrafficBlocked são true, IncomingTrafficBlocked tem prioridade.|
|incomingTrafficBlocked|Boolean|Configura o firewall para bloquear todo o tráfego de entrada independentemente de outras configurações de política. Quando IncomingTrafficRequired e IncomingTrafficBlocked são true, IncomingTrafficBlocked tem prioridade.|
|unicastResponsesToMulticastBroadcastsRequired|Boolean|Configura o firewall para permitir respostas unicast para tráfego de difusão seletiva. Quando UnicastResponsesToMulticastBroadcastsRequired e UnicastResponsesToMulticastBroadcastsBlocked são true, UnicastResponsesToMulticastBroadcastsBlocked tem prioridade.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Configura o firewall para bloquear respostas unicast para tráfego de difusão seletiva. Quando UnicastResponsesToMulticastBroadcastsRequired e UnicastResponsesToMulticastBroadcastsBlocked são true, UnicastResponsesToMulticastBroadcastsBlocked tem prioridade.|
|inboundNotificationsRequired|Boolean|Permite que o firewall exiba notificações quando um aplicativo é bloqueado de escutar em uma porta. Quando InboundNotificationsRequired e InboundNotificationsBlocked são true, InboundNotificationsBlocked tem prioridade.|
|inboundNotificationsBlocked|Boolean|Impede que o firewall exiba notificações quando um aplicativo é bloqueado de escutar em uma porta. Quando InboundNotificationsRequired e InboundNotificationsBlocked são true, InboundNotificationsBlocked tem prioridade.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Configura o firewall para mesclar regras de aplicativo autorizadas da política de grupo com as do armazenamento local, em vez de ignorar as regras de repositório local. Quando AuthorizedApplicationRulesFromGroupPolicyNotMerged e AuthorizedApplicationRulesFromGroupPolicyMerged são true, AuthorizedApplicationRulesFromGroupPolicyMerged tem prioridade.|
|authorizedApplicationRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclagem de regras de aplicativos autorizados da política de grupo com as do armazenamento local, em vez de ignorar as regras de repositório local. Quando AuthorizedApplicationRulesFromGroupPolicyNotMerged e AuthorizedApplicationRulesFromGroupPolicyMerged são true, AuthorizedApplicationRulesFromGroupPolicyMerged tem prioridade.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Configura o firewall para mesclar regras de porta globais da política de grupo com as do armazenamento local, em vez de ignorar as regras de repositório local. Quando GlobalPortRulesFromGroupPolicyNotMerged e GlobalPortRulesFromGroupPolicyMerged são true, GlobalPortRulesFromGroupPolicyMerged tem prioridade.|
|globalPortRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclagem de regras de porta global da política de grupo com as do armazenamento local, em vez de ignorar as regras de repositório local. Quando GlobalPortRulesFromGroupPolicyNotMerged e GlobalPortRulesFromGroupPolicyMerged são true, GlobalPortRulesFromGroupPolicyMerged tem prioridade.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Configura o firewall para mesclar regras de segurança de conexão da política de grupo com as do armazenamento local, em vez de ignorar as regras de repositório local. Quando ConnectionSecurityRulesFromGroupPolicyNotMerged e ConnectionSecurityRulesFromGroupPolicyMerged são true, ConnectionSecurityRulesFromGroupPolicyMerged tem prioridade.|
|connectionSecurityRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclagem de regras de segurança de conexão da política de grupo com as do armazenamento local, em vez de ignorar as regras de repositório local. Quando ConnectionSecurityRulesFromGroupPolicyNotMerged e ConnectionSecurityRulesFromGroupPolicyMerged são true, ConnectionSecurityRulesFromGroupPolicyMerged tem prioridade.|
|outboundConnectionsRequired|Boolean|Configura o firewall para permitir todas as conexões de saída por padrão. Quando OutboundConnectionsRequired e OutboundConnectionsBlocked são true, OutboundConnectionsBlocked tem prioridade.|
|outboundConnectionsBlocked|Boolean|Configura o firewall para bloquear todas as conexões de saída por padrão. Quando OutboundConnectionsRequired e OutboundConnectionsBlocked são true, OutboundConnectionsBlocked tem prioridade.|
|inboundConnectionsRequired|Boolean|Configura o firewall para permitir todas as conexões de entrada por padrão. Quando InboundConnectionsRequired e InboundConnectionsBlocked são true, InboundConnectionsBlocked tem prioridade.|
|inboundConnectionsBlocked|Boolean|Configura o firewall para bloquear todas as conexões de entrada por padrão. Quando InboundConnectionsRequired e InboundConnectionsBlocked são true, InboundConnectionsBlocked tem prioridade.|
|securedPacketExemptionAllowed|Boolean|Configura o firewall para permitir que o computador host responda ao tráfego de rede não solicitado desse tráfego é protegido por IPSec, mesmo quando stealthModeBlocked está definido como true. Quando SecuredPacketExemptionBlocked e SecuredPacketExemptionAllowed são true, SecuredPacketExemptionAllowed tem prioridade.|
|securedPacketExemptionBlocked|Boolean|Configura o firewall para bloquear o computador host para responder ao tráfego de rede não solicitado desse tráfego é protegido por IPSec, mesmo quando stealthModeBlocked está definido como true. Quando SecuredPacketExemptionBlocked e SecuredPacketExemptionAllowed são true, SecuredPacketExemptionAllowed tem prioridade.|
|policyRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar políticas de regras de firewall da política de grupo com as do armazenamento local, em vez de ignorar as regras de repositório local. Quando PolicyRulesFromGroupPolicyNotMerged e PolicyRulesFromGroupPolicyMerged são true, PolicyRulesFromGroupPolicyMerged tem prioridade.|
|policyRulesFromGroupPolicyNotMerged|Boolean|Configura o firewall para impedir a mesclagem de políticas de regras de firewall da política de grupo com as do armazenamento local, em vez de ignorar as regras de repositório local. Quando PolicyRulesFromGroupPolicyNotMerged e PolicyRulesFromGroupPolicyMerged são true, PolicyRulesFromGroupPolicyMerged tem prioridade.|

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




