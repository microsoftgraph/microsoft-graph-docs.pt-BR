---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar Microsoft Authenticator de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db534dfb13e288b82b49005b2b1a923b8bfd5112
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896638"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de usuários ou grupos habilitados para [usar](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) Microsoft Authenticator de autenticação no Azure AD.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do objeto de um usuário ou grupo do Azure AD.|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|Determina quais tipos de notificações podem ser usadas para entrar. Os valores possíveis são: `any` , ( somente sem `deviceBasedPush` senha), `push` .|
|isRegistrationRequired|Boolean|Determina se o usuário é imposto a registrar o método de autenticação. *Não há suporte para*. |
|numberMatchingRequiredState|advancedConfigState|Requer correspondência de números para notificações MFA. O valor é ignorado para notificações de login por telefone. Os valores possíveis são: `enabled`, `disabled`, `default`.|
|displayLocationInformationRequiredState|advancedConfigState|Determina se o local da assinatura deve ser mostrado ao usuário no corpo da notificação. Os valores possíveis são: `enabled`, `disabled`, `default`.|
|displayAppInformationRequiredState|advancedConfigState|Determina se o aplicativo no qual o usuário está entrando deve ser mostrado ao usuário no corpo da notificação. Os valores possíveis são: `enabled`, `disabled`, `default`.|
|targetType|authenticationMethodTargetType| Os valores possíveis são: `null`, `user`, `group`.|

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
  "numberMatchingRequiredState": "String",
  "displayLocationInformationRequiredState": "String",
  "displayAppInformationRequiredState": "String"
}

```
