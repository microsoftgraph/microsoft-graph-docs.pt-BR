---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Um conjunto de usuários ou grupos habilitados para usar a política de métodos de autenticação do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f2107ff1bde5fb34b541565e828ca91247803598
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131317"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação [do Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID do objeto de um usuário ou grupo do Azure AD.|
|isNumberMatchingRequired (Visualização Privada)|Boolean|Exigir que o usuário corresponder ao número exibido na página de login para aprovar a notificação MFA.|
|isRegistrationRequired|Boolean|Determina se o usuário é imposto a registrar o método de autenticação. *Sem suporte.* |
|shownContext (Visualização Privada)|authenticatorAppContextType|Determina quais tipos de contexto sobre a entrar devem ser mostrados para o usuário no corpo da notificação. Os valores possíveis são: `location` e `app`.|
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
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String",
  "isNumberMatchingRequired": "Boolean"
}
```

