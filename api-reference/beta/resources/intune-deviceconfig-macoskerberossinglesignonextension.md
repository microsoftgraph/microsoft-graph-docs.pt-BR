---
title: tipo de recurso macOSKerberosSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo Kerberos para dispositivos MacOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e3ffa045508c878d95ee0b7e274de69b64297aa
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199681"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a>tipo de recurso macOSKerberosSingleSignOnExtension

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um perfil de extensão de logon único de tipo Kerberos para dispositivos MacOS.


Herda de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|esfera|String|Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|domínio|Coleção de cadeias de caracteres|Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|blockAutomaticLogin|Booliano|Habilita ou desabilita o uso do chaveiro. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|CacheName|String|Obtém ou define o nome genérico dos serviços de segurança do cache Kerberos a ser usado para esse perfil. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|credentialBundleIdAccessControlList|Coleção de cadeias de caracteres|Obtém ou define uma lista de IDs de lote de aplicativos que têm permissão para acessar o tíquete de concessão de tíquete Kerberos. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|domainRealms|Coleção de cadeias de caracteres|Obtém ou define uma lista de Realms para o mapeamento do realm do domínio personalizado. Os territórios diferenciam maiúsculas de minúsculas. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|isDefaultRealm|Booliano|Quando for true, o realm deste perfil será selecionado como o padrão. Necessário se vários perfis de tipo Kerberos estiverem configurados. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordBlockModification|Booliano|Habilita ou desabilita as alterações de senha. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordExpirationDays|Int32|Substitui a expiração padrão da senha em dias. Para a maioria dos domínios, esse valor é calculado automaticamente. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordExpirationNotificationDays|Int32|Obtém ou define o número de dias até que o usuário seja notificado de que sua senha irá expirar (o padrão é 15). Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|userPrincipalName|String|Obtém ou define o nome de usuário de princípio a ser usado para esse perfil. O nome do Realm não precisa ser incluído. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordRequireActiveDirectoryComplexity|Booliano|Habilita ou desabilita se as senhas devem atender aos requisitos de complexidade do Active Directory. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordPreviousPasswordBlockCount|Int32|Obtém ou define o número de senhas anteriores para bloquear. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordMinimumLength|Int32|Obtém ou define o comprimento mínimo de uma senha. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordMinimumAgeDays|Int32|Obtém ou define o número mínimo de dias até que um usuário possa alterar sua senha novamente. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordRequirementsDescription|String|Obtém ou define uma descrição dos requisitos de complexidade de senha. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|requireUserPresence|Booliano|Obtém ou define se deve exigir autenticação por meio de ID de toque, ID de face ou uma senha para acessar a entrada de keychain. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|activeDirectorySiteCode|String|Obtém ou define o site do Active Directory. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordEnableLocalSync|Booliano|Habilita ou desabilita a sincronização de senha. Isso não afetará os usuários conectados com uma conta móvel no macOS. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|blockActiveDirectorySiteAutoDiscovery|Booliano|Habilita ou desabilita se a extensão Kerberos pode determinar automaticamente o nome do site. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|

## <a name="relationships"></a>Relações
Nenhum

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
  "blockActiveDirectorySiteAutoDiscovery": true
}
```



