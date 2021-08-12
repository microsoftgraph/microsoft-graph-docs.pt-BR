---
title: authenticationMethodConfigurations
description: objeto authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b94a80f212f7bbf4fe3f23b34828c8afec5cd3f72d7cc460ffe9455b1e2b3ae0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160097"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>tipo de recurso authenticationMethodConfiguration
Namespace: microsoft.graph

Representa uma política de método de autenticação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O nome da política.|
|state|authenticationMethodState|O estado da política. Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
