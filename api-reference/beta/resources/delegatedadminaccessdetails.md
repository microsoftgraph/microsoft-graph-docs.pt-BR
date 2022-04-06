---
title: Tipo de recurso delegatedAdminAccessDetails
description: Representa as funções administrativas que um parceiro da Microsoft tem em um locatário do cliente por meio de uma relação de administrador delegada e atribuição de acesso de administrador delegado.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a817e2f0814c19c519475d6fe4c049036ca8c3d2
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589553"
---
# <a name="delegatedadminaccessdetails-resource-type"></a>Tipo de recurso delegatedAdminAccessDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as funções administrativas que um parceiro da Microsoft tem em um locatário do cliente por meio de uma relação de administrador delegada e atribuição de acesso de administrador delegado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|unifiedRoles|[Coleção unifiedRole](../resources/unifiedrole.md)|As funções de diretório atribuídas ao parceiro microsoft no locatário do cliente.|

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

