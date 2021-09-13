---
title: Tipo de recurso controlScore
description: Esse recurso contém uma pontuação de locatário e uma descrição para um controle individual.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 155b17ed62e3aa61ea523f57ce17fd1ec0df1ee9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049534"
---
#  <a name="controlscore-resource-type"></a>Tipo de recurso controlScore

Namespace: microsoft.graph

Contém uma pontuação de locatário e uma descrição para um controle individual.

## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|controlName|Cadeia de caracteres|Controlar nome exclusivo.|
|score|Duplo|O locatário obteve pontuação para o controle (varia dia a dia, dependendo das operações do locatário no controle).|
|controlCategory|Cadeia de caracteres|Categoria de ação de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).|
|description|Cadeia de caracteres| Descrição do controle.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

