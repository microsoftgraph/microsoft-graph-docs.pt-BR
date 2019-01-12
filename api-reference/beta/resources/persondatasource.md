---
title: tipo de recurso de personDataSource
description: Representa as fontes de que dados do usuário provêm, como o diretório e os contatos do Outlook.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 540ffa81b20b40f9df2694ba634777250742daaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978498"
---
# <a name="persondatasource-resource-type"></a>tipo de recurso de personDataSource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa as fontes de que dados do usuário provêm, como o diretório e os contatos do Outlook.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|type|Cadeia de caracteres|O tipo de fonte de dados.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
