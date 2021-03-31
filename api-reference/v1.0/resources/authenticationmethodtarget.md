---
title: tipo de recurso authenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2f75a0ee81f1c43923a910bd86df4828c276706e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469105"
---
# <a name="authenticationmethodtarget-resource-type"></a>tipo de recurso authenticationMethodTarget

Namespace: microsoft.graph

Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação no Azure AD.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID do objeto de um usuário ou grupo do Azure AD.|
|isRegistrationRequired|Booliano|Determina se o usuário é imposto a registrar o método de autenticação.|
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
