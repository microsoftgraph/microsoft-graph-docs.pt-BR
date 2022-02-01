---
title: Tipo de recurso macOSKerberosSingleSignOnExtension
description: Representa um perfil de extensão único do tipo Kerberos Sign-On para dispositivos macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 945f428799ea6075a4b83028cd5daa259fcb98e6
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290578"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a>Tipo de recurso macOSKerberosSingleSignOnExtension

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um perfil de extensão único do tipo Kerberos Sign-On para dispositivos macOS.


Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|realm|Cadeia de caracteres|Obtém ou define o nome do realm que diferencia minúsculas para esse perfil.|
|domínios|String collection|Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão do aplicativo executa SSO.|
|blockAutomaticLogin|Boolean|Habilita ou desabilita o uso de chaveiro.|
|cacheName|Cadeia de caracteres|Obtém ou define o nome genérico dos Serviços de Segurança do cache Kerberos a ser usado para esse perfil.|
|credentialBundleIdAccessControlList|Conjunto de cadeias de caracteres|Obtém ou define uma lista de IDs de pacote de aplicativos permitidas para acessar o Tíquete de Concessão de Tíquete Kerberos.|
|domainRealms|Conjunto de cadeias de caracteres|Obtém ou define uma lista de realms para mapeamento de domínio personalizado. Os realms são sensíveis a casos.|
|isDefaultRealm|Booliano|Quando true, o realm desse perfil será selecionado como o padrão. Necessário se vários perfis do tipo Kerberos estão configurados.|
|passwordBlockModification|Booliano|Habilita ou desabilita alterações de senha.|
|passwordExpirationDays|Int32|Substitui a expiração de senha padrão em dias. Para a maioria dos domínios, esse valor é calculado automaticamente.|
|passwordExpirationNotificationDays|Int32|Obtém ou define o número de dias até que o usuário seja notificado de que sua senha expirará (o padrão é 15).|
|userPrincipalName|Cadeia de caracteres|Obtém ou define o nome de usuário principal a ser usado para esse perfil. O nome do realm não precisa ser incluído.|
|passwordRequireActiveDirectoryComplexity|Booliano|Habilita ou desabilita se as senhas devem atender aos requisitos de complexidade do Active Directory.|
|passwordPreviousPasswordBlockCount|Int32|Obtém ou define o número de senhas anteriores a ser bloqueado.|
|passwordMinimumLength|Int32|Obtém ou define o comprimento mínimo de uma senha.|
|passwordMinimumAgeDays|Int32|Obtém ou define o número mínimo de dias até que um usuário possa alterar sua senha novamente.|
|passwordRequirementsDescription|Cadeia de caracteres|Obtém ou define uma descrição dos requisitos de complexidade de senha.|
|requireUserPresence|Booliano|Obtém ou define se a autenticação deve ser necessária por meio de ID de Toque, ID de Face ou uma senha para acessar a entrada do chaveiro.|
|activeDirectorySiteCode|String|Obtém ou define o site do Active Directory.|
|passwordEnableLocalSync|Booliano|Habilita ou desabilita a sincronização de senha. Isso não afetará os usuários conectados com uma conta móvel no macOS.|
|blockActiveDirectorySiteAutoDiscovery|Booliano|Habilita ou desabilita se a extensão Kerberos pode determinar automaticamente seu nome de site.|
|passwordChangeUrl|Cadeia de caracteres|Obtém ou define a URL para a que o usuário será enviado quando iniciar uma alteração de senha.|
|modeCredentialUsed|Cadeia de caracteres|Selecione como outros processos usam a credencial extensão Kerberos.|
|usernameLabelCustom|Cadeia de caracteres|Esse rótulo substitui o nome de usuário mostrado na extensão Kerberos. Você pode inserir um nome para corresponder ao nome da sua empresa ou organização. Disponível para dispositivos que executam versões 11 e posteriores do macOS.|
|userSetupDelayed|Booliano|Quando definido como True, o usuário não é solicitado a configurar a extensão Kerberos até que a extensão seja habilitada pelo administrador ou um desafio Kerberos seja recebido. Disponível para dispositivos que executam versões 11 e posteriores do macOS.|
|signInHelpText|Cadeia de caracteres|Texto exibido para o usuário na janela de login Kerberos. Disponível para dispositivos que executam versões 14 e posteriores do iOS e iPadOS.|
|kerberosAppsInBundleIdACLIncluded|Booliano|Quando definida como True, a extensão Kerberos permite que todos os aplicativos inseridos com a ID do pacote de aplicativos, aplicativos gerenciados e utilitários Kerberos padrão, como TicketViewer e klist, acessem e usem a credencial. Disponível para dispositivos que executam as versões 12 e posteriores do macOS.|
|managedAppsInBundleIdACLIncluded|Booliano|Quando definida como True, a extensão Kerberos permite que aplicativos gerenciados e todos os aplicativos inseridos com a ID do pacote de aplicativos acessem a credencial. Quando definida como False, a extensão Kerberos permite que todos os aplicativos acessem a credencial. Disponível para dispositivos que executam versões 14 e posteriores do iOS e iPadOS.|
|credentialsCacheMonitored|Booliano|Quando definida como True, a credencial é solicitada no próximo desafio Kerberos correspondente ou alteração de estado de rede. Quando a credencial expira ou falta, uma nova credencial é criada. Disponível para dispositivos que executam as versões 12 e posteriores do macOS.|
|preferredKDCs|String collection|Adicionar cria uma lista ordenada de KDCs (Centros de Distribuição de Chaves) preferenciais a usar para o tráfego Kerberos. Essa lista é usada quando os servidores não podem ser descobertos usando DNS. Quando os servidores são descobertos, a lista é usada para verificações de conectividade e usada primeiro para o tráfego Kerberos. Se os servidores não responderem, o dispositivo usará a descoberta DNS. A exclusão remove uma lista existente e os dispositivos usam a descoberta DNS. Disponível para dispositivos que executam as versões 12 e posteriores do macOS.|
|tlsForLDAPRequired|Booliano|Quando definido como True, as conexões LDAP são necessárias para usar o TLS (Transport Layer Security). Disponível para dispositivos que executam versões 11 e posteriores do macOS.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": true,
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": true,
  "passwordBlockModification": true,
  "passwordExpirationDays": 1024,
  "passwordExpirationNotificationDays": 1024,
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": true,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumAgeDays": 1024,
  "passwordRequirementsDescription": "String",
  "requireUserPresence": true,
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": true,
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String",
  "modeCredentialUsed": "String",
  "usernameLabelCustom": "String",
  "userSetupDelayed": true,
  "signInHelpText": "String",
  "kerberosAppsInBundleIdACLIncluded": true,
  "managedAppsInBundleIdACLIncluded": true,
  "credentialsCacheMonitored": true,
  "preferredKDCs": [
    "String"
  ],
  "tlsForLDAPRequired": true
}
```




