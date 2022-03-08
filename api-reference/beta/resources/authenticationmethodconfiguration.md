---
title: authenticationMethodConfigurations
description: objeto authenticationMethodConfigurations.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ea0c344b1930303a34d4844a2e484fe22fae7bb9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336918"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>tipo de recurso authenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse é um tipo abstrato que representa as configurações de cada método de autenticação. Ele tem a configuração de se um método de autenticação específico está habilitado ou desabilitado para o locatário e quais usuários e grupos podem registrar e usar esse método.

Os seguintes métodos de autenticação são derivados do tipo de recurso **authenticationMethodConfiguration** :
+ [emailAuthenticationMethodConfiguration](emailauthenticationmethodconfiguration.md)
+ [fido2AuthenticationMethodConfiguration](fido2authenticationmethodconfiguration.md)
+ [microsoftAuthenticatorAuthenticationMethodConfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)
+ [smsAuthenticationMethodConfiguration](smsauthenticationmethodconfiguration.md)
+ [temporaryAccessPassAuthenticationMethodConfiguration](smsauthenticationmethodconfiguration.md)
+ [x509CertificateAuthenticationMethodConfiguration](x509certificateauthenticationmethodconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O nome da política.|
|state|authenticationMethodState|O estado da política. Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
