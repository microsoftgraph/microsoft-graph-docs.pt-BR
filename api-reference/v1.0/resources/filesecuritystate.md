---
title: Tipo de recurso fileSecurityState
description: Contém informações sobre o arquivo (não processo) relacionado ao alerta.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2db9d028c6a1550886a956bbfaad3bb3141f3141
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078858"
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
|riskScore|String|Pontuação de risco gerada/calculada pelo provedor do arquivo de alerta. Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.|

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

