---
title: Tipo de recurso teamsTabConfiguration (Tipo Aberto)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 90d9d51cffec818a601e8b7efddb4b77b1c2dc3d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052857"
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

