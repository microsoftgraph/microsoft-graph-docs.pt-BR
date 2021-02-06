---
title: Tipo de recurso authenticationMethodTarget
description: Um conjunto de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 19f8fb774ad0a60fa74d2c27655ee1174e0989af
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135447"
---
# <a name="authenticationmethodtarget-resource-type"></a>Tipo de recurso authenticationMethodTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um conjunto de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação no Azure AD.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID do objeto de um usuário ou grupo do Azure AD.|
|isRegistrationRequired|Boolean|Determina se o usuário é imposto a registrar o método de autenticação.|
|targetType|authenticationMethodTargetType|Os valores possíveis são: `user` e `group`.|
|useForSignIn|Boolean|Determina se o método de autenticação pode ser usado para entrar no Azure AD.|

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
