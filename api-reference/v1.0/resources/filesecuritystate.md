---
title: Tipo de recurso fileSecurityState
description: Contém informações sobre o arquivo (não processo) relacionado ao alerta.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ac694c40e2f8a0a126d7849cf0131f4955af27d9e96aab73c30ead2d20ad42e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218720"
---
# <a name="filesecuritystate-resource-type"></a>Tipo de recurso fileSecurityState

Namespace: microsoft.graph

Contém informações sobre o arquivo (não processo) relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Tipo complexo que contém hashes de arquivo (criptográficos e sensíveis ao local).|
|nome|Cadeia de caracteres|Nome do arquivo (sem caminho).|
|caminho|String|Caminho completo do arquivo/imageFile.|
|riskScore|Cadeia de caracteres|Pontuação de risco gerada/calculada pelo provedor do arquivo de alerta. Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.|

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

