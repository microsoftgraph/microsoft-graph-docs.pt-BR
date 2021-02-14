---
author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: O recurso UploadSession fornece informações sobre como carregar arquivos grandes para bibliotecas de documentos do OneDrive, OneDrive for Business ou SharePoint ou como anexos de arquivo para objetos de eventos e mensagens do Outlook.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0104b9349427b07ffef570d66b98720155bd7728
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239468"
---
# <a name="uploadsession-resource-type"></a>Tipo de recurso uploadSession

Namespace: microsoft.graph

O **recurso uploadSession** fornece informações sobre como carregar arquivos grandes para bibliotecas de documentos do OneDrive, OneDrive for Business ou SharePoint, ou para itens de eventos e mensagens do [Outlook](event.md) como anexos. [](message.md)

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a>Propriedades


| Propriedade       | Tipo              |Descrição
|:-------------------|:------------------|:------------------------------------
| expirationDateTime | DateTimeOffset    | Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.
| nextExpectedRanges | Coleção de cadeias de caracteres | Uma coleção de intervalos de bytes que estão ausentes do servidor para o arquivo. Estes intervalos são indexados como zero e têm o formato "início-fim" (por exemplo "0-26" para indicar os primeiros 27 bytes do arquivo). Ao carregar arquivos como anexos do Outlook, em vez de uma coleção de intervalos, essa propriedade sempre indica um único valor "{start}", o local no arquivo onde o próximo carregamento deve começar.
| uploadUrl          | String            | O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo.

## <a name="see-also"></a>Confira também

- [Anexar arquivos grandes a mensagens e eventos do Outlook como anexos ](/graph/outlook-large-attachments)
- [Carregar arquivos grandes com uma sessão de upload](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

