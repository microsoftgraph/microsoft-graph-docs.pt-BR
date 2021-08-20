---
title: " Tipo de recurso controlScore"
description: Esse recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7f5306f88f2ed14ae13cb95cee7cdb3cfe2ad569405062fe6524b8b747940b9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54190777"
---
#  <a name="controlscore-resource-type"></a>Tipo de recurso controlScore

Namespace: microsoft.graph

Esse recurso contém uma pontuação de locatário e uma descrição para um controle individual.

|Nome |Tipo |Descrição |
|:--|:--|:--|
|   controlName |   Cadeia de caracteres  |   Controlar nome exclusivo |
|   score   |   Duplo  |  O locatário obteve pontuação para o controle (varia dia a dia, dependendo das operações do locatário no controle). |
|   controlCategory |   Cadeia de caracteres  |  Categoria de ação de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura). |
|   description |   Cadeia de caracteres  |  Descrição do controle. |

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


