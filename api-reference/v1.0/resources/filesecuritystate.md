---
title: tipo de recurso filesecuritystate
description: Contém informações sobre o arquivo (não processo) relacionado ao alerta.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc9d05e875104469a25ee742635ea8e86682d9e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531424"
---
# <a name="filesecuritystate-resource-type"></a>tipo de recurso filesecuritystate

Namespace: microsoft.graph

Contém informações sobre o arquivo (não processo) relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).|
|nome|String|Nome do arquivo (sem o caminho).|
|caminho|String|Caminho completo do arquivo/ImageFile.|
|riskScore|String|Geração de um provedor/Pontuação de risco calculado do arquivo de alerta. O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.|

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
