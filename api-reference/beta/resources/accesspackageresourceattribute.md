---
title: Tipo de recurso accessPackageResourceAttribute
description: Um recurso que expõe propriedades para o solicitante de um pacote de acesso para fornecer informações personalizadas que podem ser usadas para tomar decisões de aprovação para o pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9da68399fd09b6277499985fdc87512d7a5c5ae9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861334"
---
# <a name="accesspackageresourceattribute-resource-type"></a>Tipo de recurso accessPackageResourceAttribute

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um recurso que expõe propriedades para o solicitante de um pacote de acesso para fornecer informações personalizadas que podem ser usadas para tomar decisões de aprovação para o pacote de acesso.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attributeDestination|[accessPackageResourceAttributeDestination](../resources/accesspackageresourceattributedestination.md)|Informações sobre como definir o atributo.|
|attributeName|String|O nome do atributo no sistema final.|
|attributeSource|[accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md)|Informações sobre como preencher o valor do atributo quando **um accessPackageAssignmentRequest** está sendo atendido.|
|id|String|Identificador exclusivo do atributo.|
|isEditable|String| Especifica se um valor de atributo existente pode ou não ser editado pelo solicitante.|
|isPersistedOnAssignmentRemoval|Boolean| Especifica se o atributo permanecerá no sistema final após o término de uma atribuição.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttribute",
  "attributeDestination": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
  },
  "attributeName": "String",
  "attributeSource": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeSource"
  },
  "id": "String (identifier)",
  "isEditable": "Boolean",
}
```
