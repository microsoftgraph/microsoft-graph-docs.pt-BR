---
title: Tipo de recurso fido2KeyRestrictions
description: Representa as principais restrições que são impostas como parte da política de métodos de autenticação de chaves de segurança FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a40a185f688038d3c849113ae8e9b53c4f0652f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133788"
---
# <a name="fido2keyrestrictions-resource-type"></a>Tipo de recurso fido2KeyRestrictions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as principais restrições que são impostas como parte da política de métodos de autenticação de chaves de segurança [FIDO2](../resources/fido2authenticationmethodconfiguration.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aaGuids|Coleção de cadeias de caracteres|Uma coleção de GUIDs de Atestado de Autenticador. Os AADGUIDs definem os principais tipos e fabricantes.|
|enforcementType|fido2RestrictionEnforcementType|Tipo de imposição. Os valores possíveis são: `allow` e `block`.|
|isEnforced|Boolean|Determina se a imposição de chave configurada está habilitada.|

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
