---
title: Tipo de recurso unifiedRole
description: As funções de diretório que podem ser atribuídas a um parceiro da Microsoft por meio de uma relação de administrador delegado.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 2355770dfdae2209d61903e7160527a57d4e5203
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704414"
---
# <a name="unifiedrole-resource-type"></a>Tipo de recurso unifiedRole
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As funções de diretório que podem ser atribuídas a um parceiro da Microsoft por meio de uma relação de administrador delegado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleDefinitionId|Cadeia de caracteres|A ID de definição de função unificada da função de diretório. Consulte [o recurso unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .|

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

