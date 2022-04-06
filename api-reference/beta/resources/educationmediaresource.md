---
title: Tipo de recurso educationMediaResource
description: Representa um recurso de arquivo de mídia para um educationAssignment. Herda de educationResource
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 98b645b33e2109cc187f5b895175defeb1c90d4f
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684498"
---
# <a name="educationmediaresource-resource-type"></a>Tipo de recurso educationMediaResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um recurso de arquivo de mídia para [um educationAssignment](educationassignment.md). Herda de [educationResource](educationresource.md).

Upload arquivos para o **diretório fileResource** associado à atribuição ou ao envio.

Os seguintes tipos de arquivo são recursos de mídia: , , , , `wmv`, `mp4`, `m4v`, `mpg`, `mpeg`, `m2v`, `jpg`, `png`, `gif`, `bmp`, `heic`, , `jpeg`, `mp3` `m4a``psd``avi``mkv``webm`

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|Cadeia de caracteres|Local do arquivo na pasta de ponto compartilhado. Obrigatório|
|createdBy|Cadeia de caracteres|O nome de exibição do usuário que criou esse recurso.|
|createdDateTime|DateTimeOffset|Data em que a reordenação foi adicionada.|
|displayName|string|O nome de exibição do usuário que adicionou o recurso.|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o recurso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationMediaResource"
}-->

```json
{
  "fileUrl": "String",
  "createdBy": "String (User)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": "String (User)",
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationMediaResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


