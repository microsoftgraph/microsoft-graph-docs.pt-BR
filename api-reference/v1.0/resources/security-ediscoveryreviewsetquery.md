---
title: Tipo de recurso ediscoveryReviewSetQuery
description: Representa uma consulta de conjunto de revisão, que é usada para consultar e remoção de dados armazenados em um conjunto de revisão de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 930b352d7e32b3733836e4721619492d9efe347b
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839052"
---
# <a name="ediscoveryreviewsetquery-resource-type"></a>Tipo de recurso ediscoveryReviewSetQuery

Namespace: microsoft.graph.security



Representa uma consulta de conjunto de revisão, que é usada para consultar e remoção de dados armazenados em um [conjunto de revisão de Descoberta Eletrônica](security-ediscoveryreviewset.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryReviewSetQueries](../api/security-ediscoveryreviewset-list-queries.md)|[coleção microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Obtenha uma lista dos [objetos ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) e suas propriedades.|
|[Criar ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-post-queries.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Crie um novo [objeto ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .|
|[Obter ediscoveryReviewSetQuery](../api/security-ediscoveryreviewsetquery-get.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Leia as propriedades e as relações de um [objeto ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .|
|[Atualizar ediscoveryReviewSetQuery](../api/security-ediscoveryreviewsetquery-update.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Atualize as propriedades de [um objeto ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .|
|[Excluir ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-delete-queries.md)|Nenhum|[Exclua um objeto ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md).|
|[applyTags](../api/security-ediscoveryreviewsetquery-applytags.md)|Nenhum|Aplique marcas a documentos que correspondam à consulta especificada.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| createdBy | [identitySet](/graph/api/resources/identityset) | O usuário que criou a consulta. |
| createdDateTime |DateTimeOffset| A hora e a data em que a consulta foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
| displayName | String | O nome da consulta.|
| id |String| O identificador exclusivo da consulta. Somente leitura.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | O usuário que modificou a consulta pela última vez. |
| lastModifiedDateTime |DateTimeOffset | A data e a hora em que a consulta foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
| consulta | String | A cadeia de caracteres de consulta na consulta KQL (Linguagem de Consulta de Palavra-chave). Para obter detalhes, [consulte Campos de metadados do documento na Descoberta Eletrônica (Premium)](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).  Esse campo é mapeado diretamente para a condição de palavras-chave.  Você pode refinar pesquisas usando campos listados no nome *do* campo pesquisável emparelhado com valores; por exemplo, assunto:"Finanças Trimestrais *" E Data>=01/06/2016 E Data<=01/07/2016*. |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewSetQuery",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewSetQuery",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "contentQuery": "String"
}
```

