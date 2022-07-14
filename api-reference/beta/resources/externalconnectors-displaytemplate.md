---
title: Tipo de recurso displayTemplate
description: Define a aparência do conteúdo e as condições que determinam quando o modelo deve ser exibido.
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a20b9935ad142fce0a1b1fcd2a47e608a0fec670
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788763"
---
# <a name="displaytemplate-resource-type"></a>Tipo de recurso displayTemplate

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define a aparência do conteúdo e as condições que determinam quando o modelo deve ser exibido.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de texto para o modelo de exibição; por exemplo, `contosoTickets`. Máximo de 16 caracteres. Somente caracteres alfanuméricos permitidos. |
|Layout|[microsoft.graph.Json](../resources/intune-mam-json.md)|A definição da aparência do conteúdo, representada por um [Cartão Adaptável](/adaptive-cards/authoring-cards/getting-started), que é um modelo de objeto de cartão serializado em JSON.|
|prioridade|Int32|Define a prioridade de um modelo de exibição. Um modelo de exibição com prioridade 1 é avaliado antes de um modelo com prioridade 4. Há suporte para lacunas em valores de prioridade. Deve ser um valor positivo.|
|Regras|[coleção microsoft.graph.externalConnectors.propertyRule](../resources/externalconnectors-propertyrule.md)|Especifica regras adicionais para selecionar esse modelo de exibição com base no esquema do item. Opcional.|

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