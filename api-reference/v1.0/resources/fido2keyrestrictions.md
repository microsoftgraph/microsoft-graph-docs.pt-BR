---
title: Tipo de recurso fido2KeyRestrictions
description: Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 29ec1327da2104ba14fcfb73cd4374453417f8c2c2f5cb1b10012131918f9baa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149937"
---
# <a name="fido2keyrestrictions-resource-type"></a>Tipo de recurso fido2KeyRestrictions

Namespace: microsoft.graph

Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança [FIDO2.](../resources/fido2authenticationmethodconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aaGuids|Coleção de cadeias de caracteres|Uma coleção de Authenticator GUIDs de Atestado. Os AADGUIDs definem os principais tipos e fabricantes.|
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
