---
title: Tipo de recurso crossTenantAccessPolicyTargetConfiguration
description: Define o destino de uma configuração de política de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5480a471a1114da710d9efaa859b7a6fbcb1749f
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604547"
---
# <a name="crosstenantaccesspolicytargetconfiguration-resource-type"></a>Tipo de recurso crossTenantAccessPolicyTargetConfiguration

Namespace: microsoft.graph

Define o destino de uma configuração de política de acesso entre locatários.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| accessType| crossTenantAccessPolicyTargetConfigurationAccessType | Define se o acesso é permitido ou bloqueado. Os valores possíveis são: `allowed`, `blocked`, `unknownFutureValue`. |
|targets|[Coleção crossTenantAccessPolicyTarget](../resources/crosstenantaccesspolicytarget.md)|Especifica se os usuários, grupos ou aplicativos de destino devem ser direcionados com essa regra.|

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
