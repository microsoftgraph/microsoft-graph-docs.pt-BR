---
title: tipo de recurso macOSKerberosSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo Kerberos para dispositivos MacOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99a229c78c8084ee39dafb6e87b3d6599da2a588
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955586"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a>tipo de recurso macOSKerberosSingleSignOnExtension

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um perfil de extensão de logon único de tipo Kerberos para dispositivos MacOS.


Herda de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|esfera|Cadeia de Caracteres|Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|domínio|Coleção de cadeias de caracteres|Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|blockAutomaticLogin|Boolean|Habilita ou desabilita o uso do chaveiro. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|CacheName|Cadeia de Caracteres|Obtém ou define o nome genérico dos serviços de segurança do cache Kerberos a ser usado para esse perfil. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|credentialBundleIdAccessControlList|Coleção de cadeias de caracteres|Obtém ou define uma lista de IDs de lote de aplicativos que têm permissão para acessar o tíquete de concessão de tíquete Kerberos. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|domainRealms|Coleção de cadeias de caracteres|Obtém ou define uma lista de Realms para o mapeamento do realm do domínio personalizado. Os territórios diferenciam maiúsculas de minúsculas. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|isDefaultRealm|Boolean|Quando for true, o realm deste perfil será selecionado como o padrão. Necessário se vários perfis de tipo Kerberos estiverem configurados. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordBlockModification|Boolean|Habilita ou desabilita as alterações de senha. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordExpirationDays|Int32|Substitui a expiração padrão da senha em dias. Para a maioria dos domínios, esse valor é calculado automaticamente. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordExpirationNotificationDays|Int32|Obtém ou define o número de dias até que o usuário seja notificado de que sua senha irá expirar (o padrão é 15). Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|userPrincipalName|String|Obtém ou define o nome de usuário de princípio a ser usado para esse perfil. O nome do Realm não precisa ser incluído. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordRequireActiveDirectoryComplexity|Boolean|Habilita ou desabilita se as senhas devem atender aos requisitos de complexidade do Active Directory. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordPreviousPasswordBlockCount|Int32|Obtém ou define o número de senhas anteriores para bloquear. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordMinimumLength|Int32|Obtém ou define o comprimento mínimo de uma senha. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordMinimumAgeDays|Int32|Obtém ou define o número mínimo de dias até que um usuário possa alterar sua senha novamente. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordRequirementsDescription|Cadeia de Caracteres|Obtém ou define uma descrição dos requisitos de complexidade de senha. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|requireUserPresence|Boolean|Obtém ou define se deve exigir autenticação por meio de ID de toque, ID de face ou uma senha para acessar a entrada de keychain. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|activeDirectorySiteCode|Cadeia de Caracteres|Obtém ou define o site do Active Directory. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordEnableLocalSync|Boolean|Habilita ou desabilita a sincronização de senha. Isso não afetará os usuários conectados com uma conta móvel no macOS. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|blockActiveDirectorySiteAutoDiscovery|Boolean|Habilita ou desabilita se a extensão Kerberos pode determinar automaticamente o nome do site. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordChangeUrl|Cadeia de Caracteres|Obtém ou define a URL para a qual o usuário será enviado quando iniciar uma alteração de senha. Herdado de [kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|

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
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String"
}
```



