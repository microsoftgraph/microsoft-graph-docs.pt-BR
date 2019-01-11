---
title: tipo de recurso de fileSecurityState
description: Contém informações sobre o arquivo (não process) relacionada ao alerta.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894093"
---
# <a name="filesecuritystate-resource-type"></a>tipo de recurso de fileSecurityState

Contém informações sobre o arquivo (não process) relacionada ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Tipo complexo contendo hashes de arquivo (criptográficos e confidenciais local).|
|name|Cadeia de caracteres|Nome de arquivo (sem o caminho).|
|caminho|Cadeia de caracteres|Caminho do arquivo completo do arquivo/imageFile.|
|riskScore|Cadeia de caracteres|Provedor gerado/calculado o risco de pontuação do arquivo de alerta. Valor recomendado o intervalo de 0-1, que é igual a um percentual.|

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
