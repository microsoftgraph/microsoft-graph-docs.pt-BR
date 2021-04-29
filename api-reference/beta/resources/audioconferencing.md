---
title: Tipo de recurso audioConferencing
description: Representa as informações de acesso ao telefone para uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43332de03467b4a5cf9d9cc867718ceafd8c4e82
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080145"
---
# <a name="audioconferencing-resource-type"></a>Tipo de recurso audioConferencing

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de acesso ao telefone para [um onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo              | Descrição                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| dialinUrl                   | Cadeia de Caracteres            | Uma URL para a página da Web externamente acessível que contém informações de discagem. |
| conferenceId                | Cadeia de Caracteres            | A ID da conferência da reunião online.                                       |
| tollFreeNumber (preterido) | Cadeia de Caracteres            | O número gratuito que se conecta ao Provedor de Conferência de Áudio.           |
| tollFreeNumbers             | Coleção de cadeias de caracteres | Lista de números gratuitos exibidos no convite da reunião.            |
| tollNumber (preterido)     | Cadeia de Caracteres            | O número de telefone que se conecta ao Provedor de Conferência de Áudio.                |
| tollNumbers                 | Coleção de cadeias de caracteres | Lista de números de telefone que são exibidos no convite da reunião.                 |

> [!CAUTION]
>
>- As **propriedades tollFreeNumber** **e tollNumber** são preteridas. Use as **propriedades tollFreeNumbers** **e tollNumbers.**
>- Para compatibilidade com compatibilidade, o **tollFreeNumber** original é adicionado à nova coleção **tollFreeNumbers** e o **tollNumber** original é adicionado à nova coleção **tollNumbers.**

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "conferenceId": "String",
  "tollFreeNumbers": ["String"],
  "tollNumbers": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


