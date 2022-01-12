---
title: Tipo de recurso workloadAction
description: Representa uma ação que será executada para uma carga de trabalho específica.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: fe63c772abfffb85c12d7f753c03bb6a1f168ad4
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792012"
---
# <a name="workloadaction-resource-type"></a>Tipo de recurso workloadAction

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação que será executada para uma carga de trabalho específica.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionId|String|O identificador exclusivo da ação de carga de trabalho. Obrigatório. Somente leitura.|
|category|workloadActionCategory|A categoria da ação de carga de trabalho. Os valores possíveis são: `automated`, `manual`, `unknownFutureValue`. Opcional. Somente leitura.|
|description|String|A descrição da ação de carga de trabalho. Opcional. Somente leitura.|
|displayName|String|O nome de exibição da ação de carga de trabalho. Opcional. Somente leitura.|
|service|Cadeia de caracteres|O serviço associado à ação de carga de trabalho. Opcional. Somente leitura.|
|settings|[coleção microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md)|A coleção de configurações associadas à ação de carga de trabalho. Opcional. Somente leitura.|

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
