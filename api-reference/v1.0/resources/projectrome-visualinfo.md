---
title: tipo de recurso visualInfo
description: Um tipo complexo para representar a propriedade **visualElements** no objeto Activity.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 249169ea2c640736eb544f7d9c35e44db89569ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037189"
---
# <a name="visualinfo-resource-type"></a>tipo de recurso visualInfo

Namespace: microsoft.graph

Um tipo complexo para representar a propriedade **visualElements** no objeto [Activity](../resources/projectrome-activity.md) .

Cada atividade do usuário será mostrada na linha do tempo como um cartão adaptável. Os desenvolvedores de aplicativos são incentivados a fornecer um cartão personalizado que captura a essência da atividade que ocorreu no seu aplicativo. Isso é possível ao fornecer um cartão JSON personalizado na propriedade Content.

Além dos metadados visuais com um cartão adaptável, o aplicativo pode especificar metadados de conteúdo – dados que são usados para criar inferências sobre a atividade do usuário para oferecer novas atividades para o reenvolvimento futuro. Isso é possível usando a propriedade contentInfo da atividade para fornecer um objeto JSON que aproveita as propriedades do schema.org para descrever o conteúdo.

Se um cartão personalizado não for fornecido, um cartão simples será gerado usando as propriedades displayText e Description. Os cartões personalizados são recomendados para exibir o melhor conteúdo de dentro de seu aplicativo.

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:------|:-----------|
|displayText | String | Obrigatório. Descrição de texto curto da atividade exclusiva do usuário (por exemplo, nome do documento em casos em que uma atividade refere-se à criação de documentos)|
|description | String | Opcional. Descrição de texto mais longa da atividade exclusiva do usuário (exemplo: nome do documento, primeira frase e/ou metadados)|
|CorDoFundo | String | Opcional. Cor de plano de fundo usada para renderizar a atividade na cor da marca de interface do usuário da origem do aplicativo da atividade. Deve ser uma cor hexadecimal válida|
|conteúdo | Objeto JSON não digitado | Opcional. Parte personalizada de dados-objeto JSON usado para fornecer conteúdo personalizado para renderizar a atividade na interface do usuário do shell do Windows|
|attribution | [imageInfo](../resources/projectrome-imageinfo.md) | Opcional. Objeto JSON usado para representar um ícone que representa o aplicativo usado para gerar a atividade|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

