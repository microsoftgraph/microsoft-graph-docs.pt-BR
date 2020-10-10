---
title: tipo de recurso fido2KeyRestrictions
description: Representa as restrições de chave que são impostas como parte da política de métodos de autenticação de chaves de segurança do FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c606b1d7bdbf604bd5109379bffb2c1a20f60730
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418166"
---
# <a name="fido2keyrestrictions-resource-type"></a>tipo de recurso fido2KeyRestrictions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as restrições de chave que são impostas como parte da [política de métodos de autenticação de chaves de segurança do FIDO2](../resources/fido2authenticationmethodconfiguration.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aaGuids|Conjunto de cadeias de caracteres|Uma coleção de GUIDs de atestado de autenticador. AADGUIDs definir tipos de chave e fabricantes.|
|imposiçãotype|fido2RestrictionEnforcementType|Tipo de imposição. Os valores possíveis são: `allow` e `block`.|
|isforced|Boolean|Determina se a imposição de chave configurada está habilitada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fido2KeyRestrictions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2KeyRestrictions",
  "isEnforced": "Boolean",
  "enforcementType": "String",
  "aaGuids": [
    "String"
  ]
}
```
