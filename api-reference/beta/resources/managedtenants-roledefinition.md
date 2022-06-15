---
title: Tipo de recurso roleDefinition
description: Representa informações detalhadas para a definição de função.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 6d2a34d8e6130a894341bcbbb735910c9357d3ce
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096337"
---
# <a name="roledefinition-resource-type"></a>Tipo de recurso roleDefinition

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas para a definição de função.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|A descrição da função.|
|displayName|Cadeia de caracteres|O nome de exibição da atribuição de função.|
|Templateid|String|O identificador exclusivo do modelo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.roleDefinition",
  "description": "String",
  "displayName": "String",
  "templateId": "String"
}
```
