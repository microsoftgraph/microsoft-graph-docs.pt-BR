---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar Microsoft Authenticator de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4baf2713789a54707c65fe8c2b94fe60ac275626
ms.sourcegitcommit: b7e01a1331abe5f5c9aa2828d93dad08229573f1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58336667"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de usuários ou grupos habilitados para [usar](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) Microsoft Authenticator de autenticação no Azure AD.  Herda de [authenticationMethodTarget](authenticationMethodTarget.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|Determina quais tipos de notificações podem ser usadas para entrar. Os valores possíveis são: `deviceBasedPush` (somente sem senha) `push` e `any` .|
|featureSettings|authenticatorAppFeatureSettings|Determina quais configurações adicionais devem ser aplicadas a Microsoft Authenticator. Os valores possíveis são: `requireNumberMatching` (Requer correspondência de número para notificações MFA. O valor é ignorado para notificações de login por telefone). Anulável.|
|id|Cadeia de caracteres|Identificador de objeto de um usuário ou grupo do Azure AD. Herdado da [autenticaçãoMethodTarget](authenticationmethodtarget.md).|
|isRegistrationRequired|Boolean|Determina se o usuário é imposto a registrar o método de autenticação. Herdado da [autenticaçãoMethodTarget](authenticationmethodtarget.md). *Não há suporte para*. |
|targetType|authenticationMethodTargetType| Os valores possíveis são `user`, `group` e `unknownFutureValue`. Herdado da [autenticaçãoMethodTarget](authenticationMethodTarget.md).|
<!--
|numberMatchingRequiredState|advancedConfigState|Requires number matching for MFA notifications. Value is ignored for phone sign-in notifications. Possible values are: `enabled`, `disabled`, `default`.|
|displayLocationInformationRequiredState|advancedConfigState|Determines whether the location of the sign-in should be shown to the user in the body of the notification. Possible values are: `enabled`, `disabled`, `default`.|
|displayAppInformationRequiredState|advancedConfigState|Determines whether the app the user is signing into should be shown to the user in the body of the notification. Possible values are: `enabled`, `disabled`, `default`.|
-->

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
  "featureSettings": "String"
}

```
