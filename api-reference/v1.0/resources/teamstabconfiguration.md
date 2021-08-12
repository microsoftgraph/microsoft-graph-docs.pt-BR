---
title: Tipo de recurso teamsTabConfiguration (Tipo Aberto)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7a1af503a2ba4788f22d3c7d7a76b968d1d66c167c3138ef316d056abf2f800b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196484"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>Tipo de recurso teamsTabConfiguration (Tipo Aberto)

Namespace: microsoft.graph



As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia é configurada interativamente, essas informações são definidas pelo aplicativo provedor de guias.
Além das propriedades abaixo, alguns aplicativos de provedor de guias especificam propriedades personalizadas adicionais.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|-|-|-|
|  entityId   |   string |  Identificador da entidade hospedada pelo provedor de guias.     |
|  contentUrl |   string |  URL usada para renderizar o conteúdo da guia Teams. Obrigatório.    |
|  removeUrl  |   string |  Url chamada pelo Teams cliente quando uma Guia é removida usando o Teams Client.     |
|  websiteUrl |   string |  URL para mostrar o conteúdo da guia fora do Teams.     |

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

