---
title: Tipo de recurso accessPackageResourceAttributeDestination
description: Um tipo abstrato que expõe objetos que definem o sistema final ao qual os valores configurados pelo usuário serão passados.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4d45cff09dd246affd4cc125163c8c435608b14b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61865406"
---
# <a name="accesspackageresourceattributedestination-resource-type"></a>Tipo de recurso accessPackageResourceAttributeDestination

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo abstrato usado para a **propriedade attributeDestination** de um pacote de acesso. O destino real será um subtipo desse tipo complexo.

Atualmente, o único subtipo suportado é [accessPackageUserDirectoryAttributeStore](../resources/accesspackageuserdirectoryattributestore.md).  

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeDestination"
}
```
