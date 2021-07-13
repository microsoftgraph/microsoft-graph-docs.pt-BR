---
title: Tipo de recurso workloadAction
description: Representa uma ação que será executada para uma carga de trabalho específica.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e6dbbe1458aa6dba37a26af70ee0e64b92a52cf4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401962"
---
# <a name="workloadaction-resource-type"></a>Tipo de recurso workloadAction

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que será executada para uma carga de trabalho específica.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionId|Cadeia de caracteres|O identificador exclusivo da ação de carga de trabalho. Obrigatório. Somente leitura.|
|category|workloadActionCategory|A categoria da ação de carga de trabalho. Os valores possíveis são: `automated`, `manual`, `unknownFutureValue`. Opcional. Somente leitura.|
|description|Cadeia de caracteres|A descrição da ação de carga de trabalho. Opcional. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição da ação de carga de trabalho. Opcional. Somente leitura.|
|service|Cadeia de caracteres|O serviço associado à ação de carga de trabalho. Opcional. Somente leitura.|
|configurações|[coleção microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md)|A coleção de configurações associadas à ação de carga de trabalho. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadAction",
  "actionId": "String",
  "category": "String",
  "displayName": "String",
  "description": "String",
  "service": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ]
}
```
