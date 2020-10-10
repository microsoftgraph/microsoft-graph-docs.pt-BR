---
title: tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de entrada de telefone sem senha do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a26a8fe76da954d3dc44a238665954539df0fa72
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418204"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type"></a>tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de entrada de telefone sem senha do Microsoft Authenticator] (.. /resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.

> [!NOTE]
> Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta. Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID de objeto de um usuário ou grupo do Azure AD.|
|isRegistrationRequired|Boolean|Determina se o usuário é imposto para registrar o método de autenticação.|
|shownContext|authenticatorAppContextType|Os valores possíveis são: `location` e `app`.|
|targetType|authenticationMethodTargetType|Os valores possíveis são: `user` e `group`.|
|useForSignIn|Boolean|Determina se o método de autenticação pode ser usado para entrar no Azure AD.|

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
