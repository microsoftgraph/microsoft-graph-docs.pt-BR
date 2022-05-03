---
author: nilakhan
description: Representa informações para upload de documento de impressão
title: Tipo de recurso printDocumentUploadProperties
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: 219834eb64863d67dcc6e3ed75f33bc08eead768
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176891"
---
# <a name="printdocumentuploadproperties-resource-type"></a>Tipo de recurso printDocumentUploadProperties

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o documento que está sendo carregado

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.printDocumentUploadProperties",
  "baseType": null
}-->

```json
{
  "contentType": "String",
  "documentName": "String",
  "size": "Int64",
}
```

## <a name="properties"></a>Propriedades


| Propriedade       | Tipo              |Descrição
|:-------------------|:------------------|:------------------------------------
| contentType | String    | O tipo de conteúdo do documento (MIME).
| Documentname | Cadeia de Caracteres | O nome do documento.
| size          | Int64            | O tamanho do documento em bytes.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "printDocumentUploadProperties",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
