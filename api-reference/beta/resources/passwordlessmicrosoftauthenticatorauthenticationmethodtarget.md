---
title: Tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de Login de Telefone sem Senha do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef62b251d6c943bd6290a07fa2b018bddca81ab5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872265"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type-deprecated"></a>Tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de Login de Telefone sem Senha do Microsoft Authenticator](.. /resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.

> [!CAUTION]
> A API do método de autenticação de autenticação de telefone sem senha do Microsoft Authenticator foi preterida e parou de retornar resultados em 31 de dezembro de 2020. Use a nova política [de método de autenticação do Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do objeto de um usuário ou grupo do Azure AD.|
|isRegistrationRequired|Booliano|Determina se o usuário é imposto a registrar o método de autenticação.|
|shownContext|authenticatorAppContextType|Os valores possíveis são: `location` e `app`.|
|targetType|authenticationMethodTargetType|Os valores possíveis são: `user` e `group`.|
|useForSignIn|Booliano|Determina se o método de autenticação pode ser usado para entrar no Azure AD.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String"
}
```
