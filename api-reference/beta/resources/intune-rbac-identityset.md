---
title: Tipo de recurso identitySet
description: O Conjunto de Identidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fe502776c9ab9374dcfdbb6e98ad7e379c33649f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336605"
---
# <a name="identityset-resource-type"></a>Tipo de recurso identitySet

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Conjunto de Identidade

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[identity](../resources/intune-rbac-identity.md)|A Identidade do Aplicativo. Essa propriedade é somente leitura.|
|device|[identity](../resources/intune-rbac-identity.md)|A Identidade do Dispositivo. Essa propriedade é somente leitura.|
|usuário|[identity](../resources/intune-rbac-identity.md)|A Identidade do Usuário. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identitySet",
  "application": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  },
  "user": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  }
}
```




