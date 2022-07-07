---
title: Tipo de recurso windowsWiredNetworkConfiguration
description: Essa entidade fornece descrições dos métodos, propriedades e relações declarados expostos pelo CSP de Rede Com Fio.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de125dfd9b73435ee3ebf7fd69fc2c41c4e6f81d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669501"
---
# <a name="windowswirednetworkconfiguration-resource-type"></a>Tipo de recurso windowsWiredNetworkConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa entidade fornece descrições dos métodos, propriedades e relações declarados expostos pelo CSP de Rede Com Fio.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsWiredNetworkConfigurations](../api/intune-deviceconfig-windowswirednetworkconfiguration-list.md)|[coleção windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Listar propriedades e relações dos objetos [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Obter windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-get.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Ler propriedades e relações do objeto [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Criar windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-create.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Crie um novo [objeto windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Excluir windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-delete.md)|Nenhum|Exclui um [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md).|
|[Atualizar windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-update.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Atualize as propriedades de um [objeto windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Authenticationtype|[wiredNetworkAuthenticationType](../resources/intune-deviceconfig-wirednetworkauthenticationtype.md)|Especifique se deseja autenticar o usuário, o dispositivo ou usar a autenticação de convidado (nenhuma). Se você estiver usando a autenticação de certificado, verifique se o tipo de certificado corresponde ao tipo de autenticação. Os valores possíveis são: `none`, `user`, `machine`, `machineOrUser`, `guest`. Os possíveis valores são: `none`, `user`, `machine`, `machineOrUser`, `guest`, `unknownFutureValue`.|
|cacheCredentials|Booleano|Quando TRUE, armazena em cache as credenciais do usuário no dispositivo para que os usuários não precisem continuar inserindo-as sempre que se conectarem. Quando FALSE, não armazene credenciais em cache. O valor padrão é FALSE.|
|authenticationPeriodInSeconds|Int32|Especifique o número de segundos para o cliente aguardar após uma tentativa de autenticação antes de falhar. Intervalo válido de 1 a 3600.|
|authenticationRetryDelayPeriodInSeconds|Int32|Especifique o número de segundos entre uma autenticação com falha e a próxima tentativa de autenticação. Intervalo válido de 1 a 3600.|
|eapolStartPeriodInSeconds|Int32|Especifique o número de segundos de espera antes de enviar uma mensagem inicial do EAPOL (Protocolo de Autenticação Extensível via LAN). Intervalo válido de 1 a 3600.|
|maximumEAPOLStartMessages|Int32|Especifique o número máximo de mensagens de início EAPOL (Protocolo de Autenticação Extensível via LAN) a serem enviadas antes de retornar a falha. Intervalo válido de 1 a 100.|
|maximumAuthenticationFailures|Int32|Especifique o máximo de falhas de autenticação permitidas para um conjunto de credenciais. Intervalo válido de 1 a 100.|
|enforce8021X|Booleano|Quando TRUE, o serviço de configuração automática para redes com fio requer o uso de 802.1X para autenticação de porta. Quando FALSE, 802.1X não é necessário. O valor padrão é FALSE.|
|authenticationBlockPeriodInMinutes|Int32|Especifique a duração para a qual as tentativas de autenticação automática serão impedidas de ocorrer após uma tentativa de autenticação com falha.|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Protocolo de autenticação extensível (EAP). Indica o tipo de protocolo EAP definido no ponto Wi-Fi (roteador). Os valores possíveis são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`. Os valores possíveis são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`.|
|trustedServerCertificateNames|Conjunto de cadeias de caracteres|Especifique nomes de certificado de servidor confiável.|
|Authenticationmethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Especifique o método de autenticação. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|secondaryAuthenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Especifique o método de autenticação secundário. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Especifique o protocolo de autenticação interna para EAP TTLS. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Cadeia de Caracteres|Especifique a cadeia de caracteres para substituir nomes de usuário para privacidade ao usar OAP TTLS ou PEAP.|
|performServerValidation|Booliano|Quando TRUE, habilita a verificação da identidade do servidor validando o certificado quando o tipo de EAP é selecionado como PEAP. Quando FALSE, o certificado não é validado. O valor padrão é TRUE.|
|disableUserPromptForServerValidation|Booleano|Quando TRUE, impede que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo de EAP é selecionado como PEAP. Quando FALSE, não impede que o usuário seja solicitado. O valor padrão é FALSE.|
|requireCryptographicBinding|Booleano|Quando TRUE, habilita a associação criptográfica quando o tipo EAP é selecionado como PEAP. Quando FALSE, não habilita a associação cryptogrpahic. O valor padrão é TRUE.|
|forceFIPSCompliance|Booleano|Quando VERDADEIRO, força a conformidade com FIPS. Quando FALSE, não habilita a conformidade com FIPS. O valor padrão é FALSE.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|rootCertificatesForServerValidation|[coleção windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Especifique certificados raiz para validação do servidor. Esta coleção pode conter um máximo de 500 elementos.|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Especifique o certificado de identidade para autenticação do cliente.|
|secondaryIdentityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Especifique o certificado de identidade secundário para autenticação do cliente.|
|rootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Especifique o certificado raiz para validação do cliente.|
|secondaryRootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Especifique o certificado raiz secundário para validação do cliente.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWiredNetworkConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWiredNetworkConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "authenticationType": "String",
  "cacheCredentials": true,
  "authenticationPeriodInSeconds": 1024,
  "authenticationRetryDelayPeriodInSeconds": 1024,
  "eapolStartPeriodInSeconds": 1024,
  "maximumEAPOLStartMessages": 1024,
  "maximumAuthenticationFailures": 1024,
  "enforce8021X": true,
  "authenticationBlockPeriodInMinutes": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "secondaryAuthenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "requireCryptographicBinding": true,
  "forceFIPSCompliance": true
}
```




