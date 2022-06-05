---
title: Tipo de recurso controlScore
description: Esse recurso contém uma pontuação de locatário e uma descrição para um controle individual.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 393f1323c72d6755b2947188dfcefe472b39b4ce
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898242"
---
#  <a name="controlscore-resource-type"></a>Tipo de recurso controlScore

Namespace: microsoft.graph

Contém uma pontuação de locatário e uma descrição para um controle individual.

## <a name="properties"></a>Propriedades

|Nome |Tipo |Descrição |
|:--|:--|:--|
|Controlname|Cadeia de Caracteres|Nome exclusivo do controle.|
|Pontuação|Duplo|Pontuação obtida pelo locatário para o controle (varia dia a dia, dependendo das operações de locatário no controle).|
|controlCategory|Cadeia de Caracteres|Categoria de ação de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).|
|description|String| Descrição do controle.|

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

