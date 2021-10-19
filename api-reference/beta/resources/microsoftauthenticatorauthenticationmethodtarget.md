---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar Microsoft Authenticator de autenticação.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8276f01bca86025c11eddeef21d5cce28263c379
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493477"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de usuários ou grupos habilitados para [usar](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) Microsoft Authenticator de autenticação no Azure AD.  Herda de [authenticationMethodTarget](authenticationMethodTarget.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|Determina quais tipos de notificações podem ser usadas para entrar. Os valores possíveis são: `deviceBasedPush` (somente sem senha) `push` e `any` .|
|id|Cadeia de caracteres|Identificador de objeto de um usuário ou grupo do Azure AD. Herdado da [autenticaçãoMethodTarget](authenticationmethodtarget.md).|
|isRegistrationRequired|Booliano|Determina se o usuário é imposto a registrar o método de autenticação. Herdado da [autenticaçãoMethodTarget](authenticationmethodtarget.md). *Não há suporte para*. |
|targetType|authenticationMethodTargetType| Os valores possíveis são `user`, `group` e `unknownFutureValue`. Herdado da [autenticaçãoMethodTarget](authenticationMethodTarget.md).|
|numberMatchingRequiredState|advancedConfigState|Requer correspondência de números para notificações MFA. O valor é ignorado para notificações de login por telefone. Os valores possíveis são: `enabled`, `disabled`, `default`.|
|displayAppInformationRequiredState|advancedConfigState|Determina se o usuário é mostrado contexto adicional na notificação Authenticator aplicativo. No corpo da notificação Authenticator, o usuário será mostrado no aplicativo em que está entrando, juntamente com o local de origem da solicitação de autenticação. Os valores possíveis são: `enabled`, `disabled`, `default`.|

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
  "displayAppInformationRequiredState": "String"
}

```
