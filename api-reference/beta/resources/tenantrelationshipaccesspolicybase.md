---
title: Tipo de recurso tenantRelationshipAccessPolicyBase
description: O tipo base que define uma relação de locatário.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="tenantrelationshipaccesspolicybase-resource-type"></a>Tipo de recurso tenantRelationshipAccessPolicyBase

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo base que define uma relação de locatário. Esse é um tipo abstrato herdado por objetos de política entre locatários, incluindo [crossTenantAccessPolicy](crosstenantaccesspolicy.md).

Herda de [policyBase](policybase.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| definição (preterida) | Coleção String | A definição JSON bruta da política de acesso entre locatários. **Preterido. Não use.** |
| description | String | Descrição dessa política. Obrigatório. Herdado do [policyBase](../resources/policybase.md). |
| displayName | String collection | Nome de exibição para esta política. Obrigatório. Herdado do [policyBase](../resources/policybase.md). |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantRelationshipAccessPolicyBase",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.tenantRelationshipAccessPolicyBase",
  "definition": [
    "String"
  ],
  "description": "String",
  "displayName": "String"
}
```
