---
title: Tipo de recurso reviewSetQuery
description: Representa uma consulta de conjunto de revisão, que é usada para consultar e excluir dados armazenados em um eDiscovery reviewSet.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f9c535cb1adbb62f33aee1324b6dc06a910f4b46
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445897"
---
# <a name="reviewsetquery-resource-type"></a>Tipo de recurso reviewSetQuery

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma consulta de conjunto de revisão, que é usada para consultar e excluir dados armazenados em uma revisão de descoberta [de eDiscoverySet](ediscovery-reviewset.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar consultas](../api/ediscovery-reviewsetquery-list.md) | [coleção microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | Listar as consultas de conjunto de revisão em um conjunto de revisão. |
| [Criar consultas](../api/ediscovery-reviewsetquery-post.md) | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | Crie uma nova consulta de conjunto de revisão. |
| [Obter consultas](../api/ediscovery-reviewsetquery-get.md) | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | Leia as propriedades e as relações de um **objeto reviewSetQuery.** |
| [Atualizar reviewSetQuery](../api/ediscovery-reviewsetquery-update.md) | Nenhum(a) | Atualize uma consulta de conjunto de revisão. |
| [Excluir reviewSetQuery](../api/ediscovery-reviewsetquery-delete.md) | Nenhum(a) | Excluir consulta de conjunto de revisão. |
| [applyTags](../api/ediscovery-reviewsetquery-applytags.md)|Nenhum(a)|Aplique marcas a documentos que corresponderem à consulta especificada.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| createdBy | [identitySet](/graph/api/resources/identityset) | O usuário que criou a consulta. |
| createdDateTime |DateTimeOffset| A hora e a data em que a consulta foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
| displayName | String | O nome da consulta.|
| id |String| O identificador exclusivo da consulta. Somente leitura.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | O usuário que modificou a consulta pela última vez. |
| lastModifiedDateTime |DateTimeOffset | A data e a hora em que a consulta foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
| consulta | String | A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language). Para obter detalhes, consulte [Campos de metadados de documento em Descoberta Avançada em eDiscovery](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).  Este campo mapeia diretamente para a condição de palavras-chave.  Você pode refinar pesquisas usando campos listados *no* nome de campo pesquisável emparelhados com valores; por exemplo, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSetQuery",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
