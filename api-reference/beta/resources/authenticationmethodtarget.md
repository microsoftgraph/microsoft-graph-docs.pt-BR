---
title: tipo de recurso authenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7112249f618bbda31eddeb07967d201c8b641075
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418194"
---
# <a name="authenticationmethodtarget-resource-type"></a>tipo de recurso authenticationMethodTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação no Azure AD.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID de objeto de um usuário ou grupo do Azure AD.|
|isRegistrationRequired|Boolean|Determina se o usuário é imposto para registrar o método de autenticação.|
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
