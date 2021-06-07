---
title: Tipo de recurso windowsInformationProtectionPolicy
description: Política para proteção de informações do Windows sem MDM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c8652019aa90c9c7d0558756b430d1d62de809a0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755732"
---
# <a name="windowsinformationprotectionpolicy-resource-type"></a>Tipo de recurso windowsInformationProtectionPolicy

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política para proteção de informações do Windows sem MDM


Herda de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsInformationProtectionPolicies](../api/intune-mam-windowsinformationprotectionpolicy-list.md)|Coleção [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Listar propriedades e relações dos objetos [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).|
|[Obter windowsInformationProtectionPolicy](../api/intune-mam-windowsinformationprotectionpolicy-get.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Ler propriedades e relações do objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).|
|[Criar windowsInformationProtectionPolicy](../api/intune-mam-windowsinformationprotectionpolicy-create.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Cria um novo objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).|
|[Excluir windowsInformationProtectionPolicy](../api/intune-mam-windowsinformationprotectionpolicy-delete.md)|Nenhum|Excluir um [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).|
|[Atualizar windowsInformationProtectionPolicy](../api/intune-mam-windowsinformationprotectionpolicy-update.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Atualizar as propriedades de um objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|descrição|Cadeia de caracteres|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|Nível de aplicação da WIP. Consulte a definição Enum para valores com suporte Herdados de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md). Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String|Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|enterpriseProtectedDomainNames|Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)|Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|protectionUnderLockConfigRequired|Boolean|Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados. Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|revokeOnUnenrollDisabled|Boolean|Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento. Se definido como 1 (não revogar teclas), as teclas não serão revogadas e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro. Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente. Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|rightsManagementServicesTemplateId|Guid|GUID de TemplateID para uso em criptografia RMS. O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|azureRightsManagementServicesAllowed|Boolean|Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|iconsVisible|Boolean|Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar. A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|protectedApps|Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|Os aplicativos protegidos podem acessar dados corporativos e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|exemptApps|Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos. Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados. Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|enterpriseNetworkDomainNames|Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)|Esta é a lista dos domínios que compõem os limites da empresa. Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|enterpriseProxiedDomains|Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)|Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos. As conexões com esses recursos são consideradas dados corporativos. Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80). Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|enterpriseIPRanges|Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)|Define os intervalos IP da empresa que definem os computadores da rede corporativa. Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos. Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|enterpriseIPRangesAreAuthoritative|Boolean|Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes. A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|enterpriseProxyServers|Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)|Esta é uma lista de servidores proxy. Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|enterpriseInternalProxyServers|Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)|Esta é a lista separada por vírgula de servidores proxy internos. Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59". Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet. Eles são considerados locais de rede da empresa. Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|enterpriseProxyServersAreAuthoritative|Boolean|Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho. A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|neutralDomainResources|Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)|Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|indexingEncryptedStoresOrItemsBlocked|Boolean|Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|smbAutoEncryptedFileExtensions|Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)|Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|isAssigned|Boolean|Indica se a política foi implantada a grupos de inclusão ou não. Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|revokeOnMdmHandoffDisabled|Boolean|Nova propriedade em RS2, documentação pendente|
|mdmEnrollmentUrl|String|Url do registro do MDM|
|windowsHelloForBusinessBlocked|Boolean|Valor booliano que define o Windows Hello para Empresas como um método para entrar no Windows.|
|pinMinimumLength|Int32|Valor inteiro que define o número mínimo de caracteres necessários para o PIN. O valor padrão é 4. O menor número que é possível definir para essa configuração de política é 4. O maior número que é possível definir deve ser menor que o número configurado na política de comprimento máximo do PIN ou menor que 127, seja qual for o menor.|
|pinUppercaseLetters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|Valor inteiro que configura o uso de letras maiúsculas no PIN do Windows Hello para Empresas. O padrão é NotAllow. Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinLowercaseLetters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|Valor inteiro que configura o uso de letras minúsculas no PIN do Windows Hello para Empresas. O padrão é NotAllow. Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinSpecialCharacters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|Valor inteiro que configura o uso de caracteres especiais no PIN do Windows Hello para Empresas. Os caracteres especiais válidos para o PIN do Windows Hello para Empresas incluem: ! " # $ % & ' ( ) * + , - . / : ; < = > ? @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: ` notAllow `, ` requireAtLeastOne `, ` allow'.|
|pinExpirationDays|Int32|O valor inteiro especifica o período de tempo (em dias) em que um PIN pode ser usado antes que o sistema exija que o usuário o altere. O maior número que é possível definir para essa configuração de política é 730. O menor número que é possível definir para essa configuração de política é 0. Se essa política for definida como 0, o PIN do usuário nunca irá expirar. Este nó foi adicionado no Windows 10, versão 1511. O padrão é 0.|
|numberOfPastPinsRemembered|Int32|O valor inteiro que especifica o número de PINs anteriores que podem ser associados a uma conta de usuário que não podem ser reutilizados. O maior número que é possível definir para essa configuração de política é 50. O menor número que é possível definir para essa configuração de política é 0. Se essa política for definida como 0, o armazenamento de PINs anteriores não será necessário. Este nó foi adicionado no Windows 10, versão 1511. O padrão é 0.|
|passwordMaximumAttemptCount|Int32|O número de falhas de autenticação permitido antes que o dispositivo seja apagado. O valor 0 desabilita a funcionalidade de apagamento do dispositivo. O intervalo é um inteiro X, em que 4 <= X <= 16 para desktop e 0 <= X <= 999 para dispositivos móveis.|
|minutesOfInactivityBeforeDeviceLock|Int32|Especifica a quantidade máxima de tempo (em minutos) permitida após o dispositivo ficar ocioso antes que ele seja bloqueado por PIN ou senha.   O intervalo é um inteiro X, em que 0 <= X <= 999.|
|daysWithoutContactBeforeUnenroll|Int32|Intervalo offline antes do apagamento dos dados do aplicativo (dias) |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|protectedAppLockerFiles|Coleção [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Outra maneira de inserir aplicativos protegidos por meio de arquivos xml Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|exemptAppLockerFiles|Coleção [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Outra maneira de inserir aplicativos isentos por meio de arquivos xml Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|
|assignments|Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Propriedade de navegação para lista de grupos de segurança direcionados para política. Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.ipRange"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "String",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 1024,
  "pinUppercaseLetters": "String",
  "pinLowercaseLetters": "String",
  "pinSpecialCharacters": "String",
  "pinExpirationDays": 1024,
  "numberOfPastPinsRemembered": 1024,
  "passwordMaximumAttemptCount": 1024,
  "minutesOfInactivityBeforeDeviceLock": 1024,
  "daysWithoutContactBeforeUnenroll": 1024
}
```




