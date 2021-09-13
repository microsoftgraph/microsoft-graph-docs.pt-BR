---
title: tipo de recurso authenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: efb7371c68a7e9deee9e176ebf2a69e70930e4e9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126951"
---
# <a name="authenticationmethodtarget-resource-type"></a>tipo de recurso authenticationMethodTarget

Namespace: microsoft.graph

Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação no Azure AD.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do objeto de um usuário ou grupo do Azure AD.|
|isRegistrationRequired|Boolean|Determina se o usuário é imposto a registrar o método de autenticação.|
|targetType|authenticationMethodTargetType|Os valores possíveis são: `user` e `group`.|
|useForSignIn|Booliano|Determina se o método de autenticação pode ser usado para entrar no Azure AD.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodTarget",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean"
}
```
