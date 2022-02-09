---
title: Tipo de recurso accessPackageResourceAttributeDestination
description: Um tipo abstrato que expõe objetos que definem o sistema final ao qual os valores configurados pelo usuário serão passados.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e7254c0910e930cfcb3d96fd1e4f529a6e9551c3
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468332"
---
# <a name="accesspackageresourceattributedestination-resource-type"></a>Tipo de recurso accessPackageResourceAttributeDestination

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo abstrato usado para a **propriedade attributeDestination** de [um accessPackageResourceAttribute](accesspackageresourceattribute.md). O destino real será um subtipo desse tipo complexo.

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
