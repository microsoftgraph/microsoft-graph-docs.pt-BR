---
title: Tipo de recurso searchSettings
description: Coleta todas as configurações configuráveis relacionadas ao conteúdo da pesquisa sobre o conector.
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6750ce5ea8f6b74dd55e83dae1a8f22d04ebfc15
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214913"
---
# <a name="searchsettings-resource-type"></a>Tipo de recurso searchSettings

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Coleta todas as configurações configuráveis relacionadas ao conteúdo da pesquisa sobre o conector.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|searchResultTemplates|[coleção microsoft.graph.externalConnectors.displayTemplate](../resources/externalconnectors-displaytemplate.md)|Permite que o desenvolvedor defina a aparência do conteúdo e configure condições que ditam quando o modelo deve ser exibido.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.searchSettings"
}
-->
``` json
{
  "searchResultTemplates": [
    {
      "id": "String (identifier)",
      "rules": [
        {
          "property": "itemTitle",
          "operation": "contains",
          "valuesJoinedBy": "or",
          "values": [
              "contoso",
              "smart"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "A contoso ticket."}]},
      "priority": 0
    },
        {
      "id": "String (identifier)",
      "rules": [
        {
          "property": "itemDescription",
          "operation": "contains",
          "valuesJoinedBy": "and",
          "values": [
              "contoso",
              "ticket"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "A contoso ticket."}]},
      "priority": 1
    }
  ]
}
```

