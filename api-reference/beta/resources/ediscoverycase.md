---
title: tipo de recurso ediscoveryCase
description: as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 359a74cbf48e0db2b4c3e480b73dfed928232288
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089718"
---
# <a name="ediscoverycase-resource-type"></a>tipo de recurso ediscoveryCase

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.  Saiba mais sobre casos e [descoberta eletrônica avançada](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/ediscoverycase-list.md) | coleção [ediscoveryCase](ediscoverycase.md) | Obter uma lista de ocorrências de descoberta eletrônica.|
| [Get](../api/ediscoverycase-get.md) | [ediscoveryCase](ediscoverycase.md) | Leia as propriedades do caso de descoberta eletrônica. |
| [Create](../api/ediscoverycase-post.md) | [ediscoveryCase](ediscoverycase.md) | Criar um novo **ediscoveryCase** postando na coleção cases. |
| [Update](../api/ediscoverycase-update.md) | [ediscoveryCase](ediscoverycase.md) | Atualize uma ocorrência de descoberta eletrônica. |
| [Delete](../api/ediscoverycase-delete.md) | Nenhum | Excluir uma ocorrência de descoberta eletrônica. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|closedBy|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|O usuário que fechou o caso.|
|closedDateTime|DateTimeOffset|A data e a hora em que o caso foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|createdBy|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|O usuário que criou a ocorrência.|
|createdDateTime|DateTimeOffset|A data e a hora em que a entidade foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|description|Cadeia de caracteres|A descrição do caso.|
|displayName|Cadeia de caracteres|O nome do caso.|
|externalId|Cadeia de caracteres|O número do caso externo para referência de cliente.|
|id|Cadeia de caracteres| A ID da ocorrência de descoberta eletrônica. Somente leitura. |
|lastModifiedBy|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|O último usuário que modificou a entidade.|
|lastModifiedDateTime|DateTimeOffset| A última data e hora em que a ocorrência foi modificada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|status|String| O status do caso. Os valores possíveis são:,,, `unknown` `active` `pendingDelete` `closing` `closed` , e `closedWithError` . Para obter detalhes, consulte a tabela a seguir.|

### <a name="casestatus-values"></a>valores de caseStatus

|Member|Descrição|
|:----|-----------|
| desconhecido | O status do caso é desconhecido. |
| active | O caso está ativo. |
| pendingDelete | A ocorrência foi excluída, mas a exclusão não foi totalmente transacionada. |
| Feche | O caso foi fechado, mas a operação não foi totalmente transacionada. |
| sido | O caso é fechado. |
| closedWithError | O caso está fechado, mas houve erros na liberação de isenções no caso. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Revisar conjuntos|coleção [reviewset](reviewset.md)| Coleção de conjuntos de análise no caso. Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "closedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "closedDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ediscoveryCase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


