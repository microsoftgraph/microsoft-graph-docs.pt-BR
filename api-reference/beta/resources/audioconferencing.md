---
title: Tipo de recurso audioConferencing
description: Representa as informações de acesso ao telefone para uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 98daa0db87c86625581c30e558f851d7cfa075f8
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220420"
---
# <a name="audioconferencing-resource-type"></a>Tipo de recurso audioConferencing

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de acesso ao telefone para [um onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo              | Descrição                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| dialinUrl                   | String            | Uma URL para a página da Web externamente acessível que contém informações de discagem. |
| conferenceId                | String            | A ID da conferência da reunião online.                                       |
| tollFreeNumbers             | Coleção de cadeias de caracteres | Lista de números gratuitos exibidos no convite da reunião.            |
| tollNumbers                 | Coleção de cadeias de caracteres | Lista de números de telefone que são exibidos no convite da reunião.                 |
| tollFreeNumber (preterido) | Cadeia de caracteres            | O número gratuito que se conecta ao Provedor de Conferência de Áudio.           |
| tollNumber (preterido)     | String            | O número de telefone que se conecta ao Provedor de Conferência de Áudio.                |

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
  "tollFreeNumbers": [ "String" ],
  "tollNumbers": [ "String" ]
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


