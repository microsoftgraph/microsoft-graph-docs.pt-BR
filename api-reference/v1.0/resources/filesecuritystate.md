---
title: Tipo de recurso fileSecurityState
description: Contém informações sobre o arquivo (não processo) relacionados ao alerta.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 00a8f3ce61c185969fab0adaf99483a8d03c906c
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971067"
---
# <a name="filesecuritystate-resource-type"></a>Tipo de recurso fileSecurityState

Namespace: microsoft.graph

Contém informações sobre o arquivo (não processo) relacionados ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Tipo complexo que contém hashes de arquivo (criptográficos e sensíveis à localização).|
|nome|Cadeia de caracteres|Nome do arquivo (sem caminho).|
|caminho|String|Caminho de arquivo completo do arquivo/imageFile.|
|riskScore|Cadeia de caracteres|Pontuação de risco gerada/calculada pelo provedor do arquivo de alerta. Intervalo de valor recomendado de 0 a 1, que equivale a um percentual.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

