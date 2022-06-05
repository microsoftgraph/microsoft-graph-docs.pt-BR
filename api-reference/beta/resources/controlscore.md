---
title: " Tipo de recurso controlScore"
description: Esse recurso contém uma pontuação de locatário e uma descrição para um controle individual.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: b749a81b00a1fe93c12fa5b8b17b8e7f95ca89ae
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900183"
---
#  <a name="controlscore-resource-type"></a>Tipo de recurso controlScore

Namespace: microsoft.graph

Esse recurso contém uma pontuação de locatário e uma descrição para um controle individual.

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   Controlname |   Cadeia de Caracteres  |   Nome exclusivo do controle |
|   Pontuação   |   Duplo  |  Pontuação obtida pelo locatário para o controle (varia dia a dia, dependendo das operações de locatário no controle). |
|   controlCategory |   Cadeia de Caracteres  |  Categoria de ação de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura). |
|   description |   String  |  Descrição do controle. |

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


