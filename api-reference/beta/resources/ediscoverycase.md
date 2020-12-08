---
title: tipo de recurso ediscoveryCase
description: as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 12d2901ff6a61213affd14d681c0ec7b6a74470c
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597400"
---
# <a name="ediscoverycase-resource-type"></a>tipo de recurso ediscoveryCase

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.  Saiba mais sobre casos e [descoberta eletrônica avançada](/microsoft-365/compliance/overview-ediscovery-20).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar ediscoveryCases](../api/ediscoverycase-list.md)          | coleção [ediscoveryCase](ediscoverycase.md)   | Obter uma lista de ocorrências de descoberta eletrônica.|
| [Obter ediscoveryCase](../api/ediscoverycase-get.md)            | [ediscoveryCase](ediscoverycase.md)               | Leia as propriedades do caso de descoberta eletrônica. |
| [Criar ediscoveryCase](../api/ediscoverycase-post.md)        | [ediscoveryCase](ediscoverycase.md)               | Criar um novo **ediscoveryCase** postando na coleção cases. |
| [Atualizar ediscoveryCase](../api/ediscoverycase-update.md)      | [ediscoveryCase](ediscoverycase.md)               | Atualize uma ocorrência de descoberta eletrônica. |
| [Excluir ediscoveryCase](../api/ediscoverycase-delete.md)      | Nenhum                                              | Excluir uma ocorrência de descoberta eletrônica. |
| [Fechar ediscoveryCase](../api/ediscoverycase-close.md)        | Nenhum                                              | Feche uma ocorrência de descoberta eletrônica. |
| [Reabrir ediscoveryCase](../api/ediscoverycase-reopen.md)      | Nenhum                                              | Reabra uma ocorrência de descoberta eletrônica fechada.|
| [Listar os responsáveis](../api/custodian-get.md)   | coleção [responsáveis](../resources/custodian.md) |Obtenha os recursos do responsáveis da propriedade de navegação responsáveis.|
| [Criar responsáveis](../api/ediscoverycase-post-custodians.md)  | [custódia](../resources/custodian.md)           |Criar um novo objeto de responsáveis.|
| [Listar reviewSets](../api/reviewset-list.md)   | coleção [reviewset](../resources/reviewset.md) | Obtenha os recursos reviewset da propriedade de navegação reviewSets.|
| [Criar reviewSets](../api/reviewset-post.md)  | [reviewSet](../resources/reviewset.md)           | Criar um novo objeto reviewset.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|closedBy|[identitySet](/graph/api/resources/identityset)|O usuário que fechou o caso.|
|closedDateTime|DateTimeOffset|A data e a hora em que o caso foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|createdBy|[identitySet](/graph/api/resources/identityset)|O usuário que criou a ocorrência.|
|createdDateTime|DateTimeOffset|A data e a hora em que a entidade foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|description|String|A descrição do caso.|
|displayName|String|O nome do caso.|
|externalId|Cadeia de caracteres|O número do caso externo para referência de cliente.|
|id|String| A ID da ocorrência de descoberta eletrônica. Somente leitura. |
|lastModifiedBy|[identitySet](/graph/api/resources/identityset)|O último usuário que modificou a entidade.|
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
|responsáveis|coleção [responsáveis](../resources/custodian.md)| Pessoas em uma organização que podem ter dados relevantes para o caso. |
|reviewSets|coleção [reviewset](reviewset.md)| Coleção de conjuntos de análise no caso. Somente leitura. Anulável. |

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
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "description": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
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
