---
title: Tipo de recurso unifiedRole
description: As funções de diretório que podem ser atribuídas a um parceiro da Microsoft por meio de uma relação de administrador delegada.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8a5c1cc9d450275642e767f7653eea09bcb103f6
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589579"
---
# <a name="unifiedrole-resource-type"></a>Tipo de recurso unifiedRole
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As funções de diretório que podem ser atribuídas a um parceiro da Microsoft por meio de uma relação de administrador delegada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleDefinitionId|Cadeia de caracteres|A ID de definição de função unificada da função de diretório. Consulte [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) resource.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedRole"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRole",
  "roleDefinitionId": "String"
}
```

