---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 233eed9e49ca25fafbdebc0097b513122bdb9a4b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964611"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
Namespace: microsoft.graph

Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação [do Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do objeto de um usuário ou grupo do Azure AD.|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|Determina quais tipos de notificações podem ser usadas para entrar. Os valores possíveis são: `any` , ( somente sem `deviceBasedPush` senha), `push` .|
|featureSettings|authenticatorAppFeatureSettings|Determina quais configurações adicionais devem ser aplicadas ao Microsoft Authenticator. Os valores possíveis são: `null` , `requireNumberMatching` (Requer correspondência de número para notificações MFA. O valor é ignorado para notificações de login por telefone).|
|isRegistrationRequired|Booliano|Determina se o usuário é imposto a registrar o método de autenticação. *Não há suporte para*. |
|shownContext|authenticatorAppContextType|(Visualização Privada) Determina quais tipos de contexto sobre a assinatura devem ser mostrados ao usuário no corpo da notificação. Os valores possíveis são: `location` e `app`.|
|targetType|authenticationMethodTargetType| Os valores possíveis são: `user`, `group`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "authenticationMode": "String",
  "shownContext": "String",
  "featureSettings": "String"
}
```
