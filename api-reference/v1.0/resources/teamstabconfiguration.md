---
title: tipo de recurso teamsTabConfiguration (tipo aberto)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e848fc07037dc536a116a30f1906fed3754eb05e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086400"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>tipo de recurso teamsTabConfiguration (tipo aberto)

Namespace: microsoft.graph



As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia é configurada de forma interativa, essa informação é definida pelo aplicativo de provedor de guias.
Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam Propriedades personalizadas adicionais.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|-|-|-|
|  entityId   |   string |  Identificador da entidade hospedada pelo provedor de guias.     |
|  contentUrl |   string |  URL usada para renderizar o conteúdo da guia no Microsoft Teams. Obrigatório.    |
|  removeUrl  |   string |  URL chamada pelo cliente Teams quando uma guia é removida usando o cliente Teams.     |
|  websiteUrl |   string |  URL para mostrar o conteúdo de guia fora do teams.     |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

