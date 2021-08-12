---
title: Tipo de recurso workforceIntegrationEncryption
description: Uma entidade de criptografia que define o protocolo e o segredo para uma integração de força de trabalho.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a05111fb561fe806b8b590eef321e3b7fcc9ebcd9054d2d8e5f7853e6d0c88b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180450"
---
# <a name="workforceintegrationencryption-resource-type"></a>Tipo de recurso workforceIntegrationEncryption

Namespace: microsoft.graph

Uma entidade de criptografia que define o protocolo e o segredo de [uma workforceintegration](../resources/workforceintegration.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|protocol|String| Os valores possíveis são: `sharedSecret` e `unknownFutureValue`.|
|secret|Cadeia de caracteres|Segredo compartilhado de criptografia.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
  "baseType": null
}-->

```json
{
  "protocol": "String",
  "secret": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegrationEncryption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

