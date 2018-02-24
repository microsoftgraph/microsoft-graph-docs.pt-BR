# <a name="windowsfirewallnetworkprofile-resource-type"></a>Tipo de recurso windowsFirewallNetworkProfile

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Políticas de perfil do firewall do Windows.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|firewallEnabled|Cadeia de caracteres|Ativar o firewall e a imposição de segurança avançada Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|Booliano|Impedir que o servidor funcione no modo furtivo|
|incomingTrafficBlocked|Booliano|Configura o firewall para bloquear todo o tráfego de entrada, independentemente de outras configurações de política|
|unicastResponsesToMulticastBroadcastsBlocked|Booliano|Configura o firewall para bloquear respostas unicast para tráfego de difusão multicast|
|inboundNotificationsBlocked|Booliano|Impede que o firewall exiba notificações quando um aplicativo for impedido de escutar em uma porta|
|authorizedApplicationRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar regras de aplicativos autorizados da política de grupo com as regras do armazenamento local, em vez de ignorar as regras do armazenamento local|
|globalPortRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar regras globais da porta da política de grupo com as regras do armazenamento local, em vez de ignorar as regras do armazenamento local|
|connectionSecurityRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar regras de segurança da conexão da política de grupo com as regras do armazenamento local, em vez de ignorar as regras do armazenamento local|
|outboundConnectionsBlocked|Booliano|Configura o firewall para bloquear todas as conexões de saída por padrão|
|inboundConnectionsBlocked|Booliano|Configura o firewall para bloquear todas as conexões de entrada por padrão|
|securedPacketExemptionAllowed|Booliano|Configura o firewall para permitir que o computador host responda ao tráfego de rede não solicitado protegido por IPSec mesmo quando stealthModeBlocked for definido como true|
|policyRulesFromGroupPolicyMerged|Booliano|Configura o firewall para mesclar regras do firewall da política de grupo com as regras do armazenamento local, em vez de ignorar as regras do armazenamento local|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
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



