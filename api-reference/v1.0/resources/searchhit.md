---
title: Tipo de recurso searchHit
description: Descrição da entidade searchHit
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 487fbee4e501b6d4154b1ed08102730fd278730c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878824"
---
# <a name="searchhit-resource-type"></a>Tipo de recurso searchHit

Namespace: microsoft.graph

Representa um único resultado na lista de resultados da pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|contentSource|Cadeia de caracteres|O nome da fonte de conteúdo da **qual o externalItem** faz parte .|
|hitId|String|O identificador interno do item.|
|classificação|Int32|A classificação ou a ordem do resultado.|
|resultTemplateId|String|ID do modelo de resultado usado para renderizar o resultado da pesquisa. Essa ID deve mapear para um layout de exibição no dicionário **resultTemplates** que também está incluído na [searchResponse](searchresponse.md).|
|recurso|[entity](entity.md)|A representação básica da Microsoft Graph do resultado da pesquisa.|
|summary|String|Um resumo do resultado, se um resumo estiver disponível.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "contentSource": "String",
  "hitId": "String",
  "rank": "Int32",
  "resultTemplateId": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

