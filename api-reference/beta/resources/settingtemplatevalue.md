---
title: Tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.
localization_priority: Normal
ms.openlocfilehash: e941630ab72363db1c4be40079cf2af9e40ff002
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811862"
---
# <a name="settingtemplatevalue-resource-type"></a>Tipo de recurso settingTemplateValue

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|defaultValue|string|Valor padrão para a configuração. Somente leitura.|
|description|string|Descrição da configuração. Somente leitura.|
|name|string|Nome da configuração. Somente leitura.|
|type|string|Tipo da configuração. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
