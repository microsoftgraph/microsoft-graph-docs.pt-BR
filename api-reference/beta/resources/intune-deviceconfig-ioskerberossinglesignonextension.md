---
title: Tipo de recurso iosKerberosSingleSignOnExtension
description: Representa um perfil de extensão único do tipo Kerberos Sign-On para dispositivos iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90cca5e1488ce4fff9742099209b3e3e03bf5716
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347393"
---
# <a name="ioskerberossinglesignonextension-resource-type"></a>Tipo de recurso iosKerberosSingleSignOnExtension

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um perfil de extensão único do tipo Kerberos Sign-On para dispositivos iOS.


Herda de [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|realm|String|Obtém ou define o nome do realm que diferencia minúsculas para esse perfil.|
|domínios|Coleção de cadeias de caracteres|Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão do aplicativo executa SSO.|
|blockAutomaticLogin|Boolean|Habilita ou desabilita o uso de chaveiro.|
|cacheName|String|Obtém ou define o nome genérico dos Serviços de Segurança do cache Kerberos a ser usado para esse perfil.|
|credentialBundleIdAccessControlList|Coleção de cadeias de caracteres|Obtém ou define uma lista de IDs de pacote de aplicativos permitidas para acessar o Tíquete de Concessão de Tíquete Kerberos.|
|domainRealms|Coleção de cadeias de caracteres|Obtém ou define uma lista de realms para mapeamento de domínio personalizado. Os realms são sensíveis a casos.|
|isDefaultRealm|Boolean|Quando true, o realm desse perfil será selecionado como o padrão. Necessário se vários perfis do tipo Kerberos estão configurados.|
|passwordBlockModification|Boolean|Habilita ou desabilita alterações de senha.|
|passwordExpirationDays|Int32|Substitui a expiração de senha padrão em dias. Para a maioria dos domínios, esse valor é calculado automaticamente.|
|passwordExpirationNotificationDays|Int32|Obtém ou define o número de dias até que o usuário seja notificado de que sua senha expirará (o padrão é 15).|
|userPrincipalName|String|Obtém ou define o nome de usuário principal a ser usado para esse perfil. O nome do realm não precisa ser incluído.|
|passwordRequireActiveDirectoryComplexity|Booliano|Habilita ou desabilita se as senhas devem atender aos requisitos de complexidade do Active Directory.|
|passwordPreviousPasswordBlockCount|Int32|Obtém ou define o número de senhas anteriores a ser bloqueado.|
|passwordMinimumLength|Int32|Obtém ou define o comprimento mínimo de uma senha.|
|passwordMinimumAgeDays|Int32|Obtém ou define o número mínimo de dias até que um usuário possa alterar sua senha novamente.|
|passwordRequirementsDescription|String|Obtém ou define uma descrição dos requisitos de complexidade de senha.|
|requireUserPresence|Boolean|Obtém ou define se a autenticação deve ser necessária por meio de ID de Toque, ID de Face ou uma senha para acessar a entrada do chaveiro.|
|activeDirectorySiteCode|String|Obtém ou define o site do Active Directory.|
|passwordEnableLocalSync|Boolean|Habilita ou desabilita a sincronização de senha. Isso não afetará os usuários conectados com uma conta móvel no macOS.|
|blockActiveDirectorySiteAutoDiscovery|Boolean|Habilita ou desabilita se a extensão Kerberos pode determinar automaticamente seu nome de site.|
|passwordChangeUrl|String|Obtém ou define a URL para a que o usuário será enviado quando iniciar uma alteração de senha.|
|signInHelpText|String|Texto exibido para o usuário na janela de login Kerberos. Disponível para dispositivos que executam versões 14 e posteriores do iOS e iPadOS.|
|managedAppsInBundleIdACLIncluded|Booliano|Quando definida como True, a extensão Kerberos permite que aplicativos gerenciados e todos os aplicativos inseridos com a ID do pacote de aplicativos acessem a credencial. Quando definida como False, a extensão Kerberos permite que todos os aplicativos acessem a credencial. Disponível para dispositivos que executam versões 14 e posteriores do iOS e iPadOS.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosKerberosSingleSignOnExtension",
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
  "signInHelpText": "String",
  "managedAppsInBundleIdACLIncluded": true
}
```




