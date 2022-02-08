---
title: Tipo de recurso crossTenantAccessPolicyTargetConfiguration
description: Define o destino de uma configuração de configuração de política de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicytargetconfiguration-resource-type"></a>Tipo de recurso crossTenantAccessPolicyTargetConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o destino de uma configuração de configuração de política de acesso entre locatários.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| accessType| crossTenantAccessPolicyTargetConfigurationAccessType | Define se o acesso é permitido ou bloqueado. Os valores possíveis são: `allowed`, `blocked`, `unknownFutureValue`. |
|targets|[Coleção crossTenantAccessPolicyTarget](../resources/crosstenantaccesspolicytarget.md)|Especifica se os usuários, grupos ou aplicativos de destino serão destinados a essa regra.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyTargetConfiguration",
  "accessType": "String",
  "targets": [
    {
      "@odata.type": "microsoft.graph.crossTenantAccessPolicyTarget"
    }
  ]
}
```
