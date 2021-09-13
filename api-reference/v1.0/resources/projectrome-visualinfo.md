---
title: Tipo de recurso visualInfo
description: Um tipo complexo para representar a **propriedade visualElements** no objeto activity.
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 3c71a3613c51c1b7494fd44550108d8cd63645ff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019185"
---
# <a name="visualinfo-resource-type"></a>Tipo de recurso visualInfo

Namespace: microsoft.graph

Um tipo complexo para representar a **propriedade visualElements** no [objeto activity.](../resources/projectrome-activity.md)

Cada atividade do usuário será mostrada em Linha do Tempo como um Cartão Adaptável. Os desenvolvedores de aplicativos são incentivados a fornecer um Cartão personalizado que captura a essência da atividade que ocorreu em seu aplicativo. Isso é possível fornecendo um cartão JSON personalizado na propriedade de conteúdo.

Além dos metadados visuais com um Cartão Adaptável, o aplicativo pode especificar metadados de conteúdo – dados que serão usados para criar inferências sobre a atividade do usuário, a fim de oferecer novas atividades para futuras re-envolvimentos. Isso é possível usando a propriedade contentInfo da atividade para fornecer um objeto JSON que utiliza schema.org propriedades para descrever o conteúdo.

Se um cartão personalizado não for fornecido, um cartão simples será gerado usando as propriedades displayText e description. Os cartões personalizados são recomendados para mostrar o melhor conteúdo de dentro do seu aplicativo.

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:------|:-----------|
|displayText | Cadeia de caracteres | Obrigatório. Breve descrição de texto da atividade exclusiva do usuário (por exemplo, nome do documento nos casos em que uma atividade se refere à criação de documento)|
|description | String | Opcional. Descrição de texto mais longa da atividade exclusiva do usuário (exemplo: nome do documento, primeira frase e/ou metadados)|
|backgroundColor | String | Opcional. Cor de plano de fundo usada para renderizar a atividade na interface do usuário - cor da marca para a origem do aplicativo da atividade. Deve ser uma cor hexaxa válida|
|conteúdo | Objeto JSON sem tipo | Opcional. Parte personalizada de dados - objeto JSON usado para fornecer conteúdo personalizado para renderizar a atividade na interface do usuário Windows Shell|
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

