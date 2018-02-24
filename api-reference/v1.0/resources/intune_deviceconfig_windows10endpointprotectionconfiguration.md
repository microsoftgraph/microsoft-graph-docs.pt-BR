# <a name="windows10endpointprotectionconfiguration-resource-type"></a>Tipo de recurso windows10EndpointProtectionConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso Windows10EndpointProtectionConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10EndpointProtectionConfigurations](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_list.md)|Coleção [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Listar propriedades e relações dos objetos [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[Obter windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_get.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Ler propriedades e relações do objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[Criar windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_create.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[Excluir windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_delete.md)|Nenhum|Excluir um [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[Atualizar windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_update.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Última modificação de DateTime do objeto. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|firewallBlockStatefulFTP|Booliano|Bloqueia conexões de FTP com estado ao dispositivo|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive. Após esse período, as associações de segurança expirarão e serão excluídas. Valores válidos de 300 a 3.600|
|firewallPreSharedKeyEncodingMethod|Cadeia de caracteres|Selecione a codificação de chave pré compartilhada a ser usada Os valores possíveis são: `deviceDefault`, `none`, `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Booliano|Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos|
|firewallIPSecExemptionsAllowICMP|Booliano|Configura isenções IPSec para permitir que ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Booliano|Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores|
|firewallIPSecExemptionsAllowDHCP|Booliano|Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6|
|firewallCertificateRevocationListCheckMethod|Cadeia de caracteres|Especifique como a lista de revogação de certificados é aplicada Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Booliano|Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto|
|firewallPacketQueueingMethod|Cadeia de caracteres|Configura como o enfileiramento de pacote deve aplicado no cenário de gateway de túnel Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes do domínio|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes públicas|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Define as configurações de perfil de firewall das redes privadas|
|defenderAttackSurfaceReductionExcludedPaths|Coleção String|Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque|
|defenderGuardedFoldersAllowedAppPaths|Coleção String|Lista de caminhos para exe com permissão para acessar as pastas protegidas|
|defenderAdditionalGuardedFolders|Coleção String|Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas|
|defenderExploitProtectionXml|Binária|Conteúdo XML com informações sobre a proteção contra vulnerabilidades.|
|defenderExploitProtectionXmlFileName|Cadeia de caracteres|Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.|
|defenderSecurityCenterBlockExploitProtectionOverride|Booliano|Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.|
|appLockerApplicationControl|Cadeia de caracteres|Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos. Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|smartScreenEnableInShell|Booliano|Permite que os administradores de TI configurem SmartScreen para Windows.|
|smartScreenBlockOverrideForFiles|Booliano|Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.|
|applicationGuardEnabled|Booliano|Habilitar o Windows Defender Application Guard|
|applicationGuardBlockFileTransfer|Cadeia de caracteres|Impedir a área de transferência de transferir arquivo de imagem, arquivo de texto ou ambos Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Booliano|Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros|
|applicationGuardAllowPersistence|Booliano|Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web etc.)|
|applicationGuardForceAuditing|Booliano|A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema etc.)|
|applicationGuardBlockClipboardSharing|Cadeia de caracteres|Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções. Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Booliano|Permitir a impressão em PDF pelo contêiner|
|applicationGuardAllowPrintToXPS|Booliano|Permitir a impressão em XPS pelo contêiner|
|applicationGuardAllowPrintToLocalPrinters|Booliano|Permitir a impressão em impressoras locais pelo contêiner|
|applicationGuardAllowPrintToNetworkPrinters|Booliano|Permitir a impressão em impressoras da rede pelo contêiner|
|bitLockerDisableWarningForOtherDiskEncryption|Booliano|Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.|
|bitLockerEnableStorageCardEncryptionOnMobile|Booliano|Permite que o administrador exija que a criptografia seja ativada usando BitLocker. Essa política é válida apenas para uma SKU móvel.|
|bitLockerEncryptDevice|Booliano|Permite que o administrador exija que a criptografia seja ativada usando BitLocker.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|Política da unidade removível do BitLocker.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status da instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
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
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
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
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
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
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```



