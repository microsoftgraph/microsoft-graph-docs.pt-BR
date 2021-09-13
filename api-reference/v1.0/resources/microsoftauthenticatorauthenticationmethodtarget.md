---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar Microsoft Authenticator de autenticação.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 810403eff5801ebcbafd56cf3de6252fe1f68bf8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067077"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
Namespace: microsoft.graph

Uma coleção de usuários ou grupos habilitados para [usar](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) Microsoft Authenticator de autenticação no Azure AD.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do objeto de um usuário ou grupo do Azure AD.|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|Determina quais tipos de notificações podem ser usadas para entrar. Os valores possíveis são: `any` , ( somente sem `deviceBasedPush` senha), `push` .|
|featureSettings|authenticatorAppFeatureSettings|Determina quais configurações adicionais devem ser aplicadas a Microsoft Authenticator. Os valores possíveis são: `null` , `requireNumberMatching` (Requer correspondência de número para notificações MFA. O valor é ignorado para notificações de login por telefone).|
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
