# <a name="windowsfirewallnetworkprofile-resource-type"></a>Tipo de recurso windowsFirewallNetworkProfile

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Políticas de perfil do firewall do Windows.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Configura o dispositivo host para permitir ou bloquear o firewall e imposição de segurança avançada para o perfil de rede. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|Booleano|Impede que o servidor funcione no modo furtivo Quando StealthModeRequired e StealthModeBlocked são ambos true, StealthModeBlocked tem prioridade.|
|incomingTrafficBlocked|Booleano|Configura o firewall para bloquear todo o tráfego de entrada independentemente das outras configurações de política. Quando IncomingTrafficRequired e IncomingTrafficBlocked são ambos true, IncomingTrafficBlocked tem prioridade.|
|unicastResponsesToMulticastBroadcastsBlocked|Booleano|Configura o firewall para bloquear respostas unicast para tráfego de difusão seletiva. Quando UnicastResponsesToMulticastBroadcastsRequired e UnicastResponsesToMulticastBroadcastsBlocked são ambos true, UnicastResponsesToMulticastBroadcastsBlocked tem prioridade.|
|inboundNotificationsBlocked|Booleano|Impede que o firewall exiba notificações quando um aplicativo for impedido de escutar em uma porta. Quando InboundNotificationsRequired e InboundNotificationsBlocked são ambos true, InboundNotificationsBlocked tem prioridade.|
|authorizedApplicationRulesFromGroupPolicyMerged|Booleano|Configura o firewall para mesclar regras de aplicativos autorizados pela política de grupo com as regras do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando AuthorizedApplicationRulesFromGroupPolicyNotMerged e AuthorizedApplicationRulesFromGroupPolicyMerged são ambas true, AuthorizedApplicationRulesFromGroupPolicyMerged tem prioridade.|
|globalPortRulesFromGroupPolicyMerged|Booleano|Configura o firewall para mesclar regras globais da porta definidas pela política de grupo com as regras do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando GlobalPortRulesFromGroupPolicyNotMerged e GlobalPortRulesFromGroupPolicyMerged são ambas true, GlobalPortRulesFromGroupPolicyMerged tem prioridade.|
|connectionSecurityRulesFromGroupPolicyMerged|Booleano|Configura o firewall para mesclar regras de segurança de conexão definidas pela política de grupo com as regras do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando ConnectionSecurityRulesFromGroupPolicyNotMerged e ConnectionSecurityRulesFromGroupPolicyMerged são ambas true, ConnectionSecurityRulesFromGroupPolicyMerged tem prioridade.|
|outboundConnectionsBlocked|Booleano|Configura o firewall para bloquear todas as conexões de saída por padrão. Quando OutboundConnectionsRequired e OutboundConnectionsBlocked são ambas true, OutboundConnectionsBlocked tem prioridade.|
|inboundConnectionsBlocked|Booleano|Configura o firewall para bloquear todas as conexões de entrada por padrão. Quando InboundConnectionsRequired e InboundConnectionsBlocked são ambas true, InboundConnectionsBlocked tem prioridade.|
|securedPacketExemptionAllowed|Booleano|Configura o firewall para permitir que o computador host responda ao tráfego de rede não solicitado protegido por IPSec mesmo quando stealthModeBlocked for definido como true. Quando SecuredPacketExemptionBlocked e SecuredPacketExemptionAllowed são ambos true, SecuredPacketExemptionAllowed tem prioridade.|
|policyRulesFromGroupPolicyMerged|Booleano|Configura o firewall para mesclar regras da política de firewall definidas pela política de grupo com as regras do armazenamento local, em vez de ignorar as regras do armazenamento local. Quando PolicyRulesFromGroupPolicyNotMerged e PolicyRulesFromGroupPolicyMerged são ambos true, PolicyRulesFromGroupPolicyMerged tem prioridade.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeBlocked": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "policyRulesFromGroupPolicyMerged": true
}
```








