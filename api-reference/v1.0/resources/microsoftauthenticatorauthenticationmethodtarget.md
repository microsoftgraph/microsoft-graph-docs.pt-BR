---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 43c8e5a4ba92e838a64ec5f345ae82c744b53dee
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469245"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
Namespace: microsoft.graph

Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação [do Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID do objeto de um usuário ou grupo do Azure AD.|
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
