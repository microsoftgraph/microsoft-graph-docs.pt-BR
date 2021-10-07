---
title: Tipo de recurso educationMediaResource
description: Representa um recurso de arquivo de mídia para um educationAssignment. Herda de educationResource
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d89835234ff1e388b5da9c618322ebad0c8a101e
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220789"
---
# <a name="educationmediaresource-resource-type"></a>Tipo de recurso educationMediaResource

Namespace: microsoft.graph

Representa um recurso de arquivo de mídia para [um educationAssignment](educationassignment.md). Herda de [educationResource](educationresource.md).

Upload esses arquivos para o **diretório fileResource** associado à atribuição ou envio.

Os seguintes tipos de arquivo são recursos de mídia: `webm` , , , , , , , `mkv` , `avi` , , , `wmv` , , `mp4` `m4v` e `mpg` `mpeg` `m2v` `jpg` `png` `gif` `bmp` `heic` `jpeg` `psd` `mp3` `m4a` .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|Cadeia de caracteres|Local do arquivo na pasta de ponto compartilhado. Obrigatório|

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
  "fileUrl": "String"
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


