---
title: Tipo de recurso fido2KeyRestrictions
description: Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c1781e39952bb3bf7cfb307d06ca3167ff58a2a6
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469448"
---
# <a name="fido2keyrestrictions-resource-type"></a>Tipo de recurso fido2KeyRestrictions

Namespace: microsoft.graph

Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança [FIDO2.](../resources/fido2authenticationmethodconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aaGuids|Coleção de cadeias de caracteres|Uma coleção de GUIDs de Atestado do Autenticador. Os AADGUIDs definem os principais tipos e fabricantes.|
|enforcementType|fido2RestrictionEnforcementType|Tipo de imposição. Os valores possíveis são: `allow` e `block`.|
|isEnforced|Booliano|Determina se a imposição de chave configurada está habilitada.|

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
