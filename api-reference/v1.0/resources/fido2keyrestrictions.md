---
title: Tipo de recurso fido2KeyRestrictions
description: Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança FIDO2.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 37b9e2c7a66b3ce9a43c08560f5e5f4a8e0acc2e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036526"
---
# <a name="fido2keyrestrictions-resource-type"></a>Tipo de recurso fido2KeyRestrictions

Namespace: microsoft.graph

Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança [FIDO2.](../resources/fido2authenticationmethodconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aaGuids|Coleção String|Uma coleção de Authenticator GUIDs de Atestado. Os AADGUIDs definem os principais tipos e fabricantes.|
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
