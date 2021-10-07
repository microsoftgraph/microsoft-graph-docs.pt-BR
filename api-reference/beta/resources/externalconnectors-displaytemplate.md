---
title: Tipo de recurso displayTemplate
description: Define a aparência do conteúdo e as condições que ditam quando o modelo deve ser exibido.
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5138bb43bea3aec216dcb86ffc2f09eaec96e315
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214915"
---
# <a name="displaytemplate-resource-type"></a>Tipo de recurso displayTemplate

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define a aparência do conteúdo e as condições que ditam quando o modelo deve ser exibido.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de texto do modelo de exibição; por exemplo, `contosoTickets` .|
|layout|[microsoft.graph.Json](../resources/intune-mam-json.md)|A definição da aparência do conteúdo, representada por um [Cartão Adaptável](https://docs.microsoft.com/adaptive-cards/authoring-cards/getting-started), que é um modelo de objeto de cartão serializado JSON.|
|prioridade|Int32|Define a prioridade de um modelo de exibição. Um modelo de exibição com prioridade 1 é avaliado antes de um modelo com prioridade 4. Há suporte para lacunas nos valores de prioridade.|
|rules|[coleção microsoft.graph.externalConnectors.propertyRule](../resources/externalconnectors-propertyrule.md)|Especifica regras adicionais para selecionar esse modelo de exibição com base no esquema do item. Opcional.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.displayTemplate"
}
-->
``` json
    {
      "id": "String",
      "rules": [
        {
          "property": "String",
          "operation": "String",
          "valuesJoinedBy": "String",
          "values": [
              "String",
              "String"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "String"}]},
      "priority": 0
    }
```

