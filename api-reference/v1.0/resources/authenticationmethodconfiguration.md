---
title: authenticationMethodConfigurations
description: objeto authenticationMethodConfigurations.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b7dee4297fb00dd54e9f9b8edf19da00c866a0f4
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2022
ms.locfileid: "62238970"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>tipo de recurso authenticationMethodConfiguration
Namespace: microsoft.graph

Esse é um tipo abstrato que representa as configurações de cada método de autenticação. Ele tem a configuração de se um método de autenticação específico está habilitado ou desabilitado para o locatário e quais usuários e grupos podem registrar e usar esse método.

Os seguintes métodos de autenticação são derivados do tipo de recurso **authenticationMethodConfiguration:**
+ [emailAuthenticationMethodConfiguration](emailauthenticationmethodconfiguration.md)
+ [fido2AuthenticationMethodConfiguration](fido2authenticationmethodconfiguration.md)
+ [microsoftAuthenticatorAuthenticationMethodConfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O nome da política.|
|estado|authenticationMethodState|O estado da política. Os valores possíveis são: `enabled`, `disabled`.|

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
