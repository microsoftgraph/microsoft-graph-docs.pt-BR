---
author: JeremyKelley
description: Representa informações de um processo interativo para carregar arquivos grandes para o OneDrive, o OneDrive for Business ou bibliotecas de documentos do SharePoint, ou como anexos de arquivo para objetos de mensagem do Outlook.
title: tipo de recurso uploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 43086486175add54a7fe809eb9dffb8b3747c92a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519572"
---
# <a name="uploadsession-resource-type"></a>tipo de recurso uploadSession

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações de um processo interativo para carregar arquivos grandes para o OneDrive, o OneDrive for Business ou bibliotecas de documentos do SharePoint, ou para objetos de [mensagem](message.md) do Outlook como anexos.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession",
  "baseType": null
}-->

```json
{
  "uploadUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "nextExpectedRanges": ["String"]
}
```

## <a name="properties"></a>Propriedades


| Propriedade       | Tipo              |Descrição
|:-------------------|:------------------|:------------------------------------
| expirationDateTime | DateTimeOffset    | Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.
| nextExpectedRanges | Coleção de cadeias de caracteres | Ao carregar arquivos em bibliotecas de documentos, esta é uma coleção de intervalos de bytes que o servidor está faltando para o arquivo. Esses intervalos são indexados por zero e do formato, "{Start}-{End}" (por exemplo, "0-26" para indicar os primeiros 27 bytes do arquivo). Ao carregar arquivos como anexos de mensagem do Outlook, em vez de uma coleção de intervalos, essa propriedade sempre indica um valor único "{Start}", o local no arquivo em que o próximo carregamento deve começar.
| uploadUrl          | String            | O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo.

## <a name="see-also"></a>Confira também

- [Anexar arquivos grandes às mensagens do Outlook como anexos](/graph/outlook-large-attachments)
- [Carregar arquivos grandes com uma sessão de upload](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": []
}
-->
