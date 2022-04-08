---
title: Tipo de recurso delegatedAdminAccessDetails
description: Representa as funções administrativas que um parceiro da Microsoft tem em um locatário do cliente por meio de uma relação de administrador delegado e atribuição de acesso de administrador delegado.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: c67f7792ea1124228a23fdc5b642dc3de47739a8
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704155"
---
# <a name="delegatedadminaccessdetails-resource-type"></a>Tipo de recurso delegatedAdminAccessDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as funções administrativas que um parceiro da Microsoft tem em um locatário do cliente por meio de uma relação de administrador delegado e atribuição de acesso de administrador delegado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|unifiedRoles|[coleção unifiedRole](../resources/unifiedrole.md)|As funções de diretório atribuídas pelo parceiro da Microsoft no locatário do cliente.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessDetails",
  "unifiedRoles": [
    {
      "@odata.type": "microsoft.graph.unifiedRole"
    }
  ]
}
```

