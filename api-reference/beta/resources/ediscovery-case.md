---
title: tipo de recurso case
description: No contexto da Descoberta eDiscovery, contém custodiantes, regiões, coleções, conjuntos de revisão e exportações.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f1acccc8b6fd297827386c43829b731fcf5c8475
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60449450"
---
# <a name="case-resource-type"></a>tipo de recurso case

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No contexto da Descoberta eDiscovery, contém custodiantes, regiões, coleções, conjuntos de revisão e exportações. Para obter detalhes, [consulte Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20).

>[!NOTE]
>A partir de setembro de 2021, as operações POST criarão casos grandes. Para saber mais sobre casos grandes, consulte [Use large cases in Advanced eDiscovery](/microsoft-365/compliance/advanced-ediscovery-large-cases). Para obter detalhes, consulte a [postagem do](https://go.microsoft.com/fwlink/?linkid=2172604) blog Alterações na descoberta Microsoft 365 criar API de caso avançada.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar casos](../api/ediscovery-case-list.md) | [coleção microsoft.graph.ediscovery.case](ediscovery-case.md) | Recupere uma lista de [objetos case.](../resources/ediscovery-case.md)|
| [Criar caso](../api/ediscovery-case-post.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | Crie um novo **objeto case.** |
| [Obter caso](../api/ediscovery-case-get.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | Recupere as propriedades e as relações de um **objeto case.** |
| [Caso de atualização](../api/ediscovery-case-update.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | Atualize as propriedades de um **objeto case.** |
| [Excluir caso](../api/ediscovery-case-delete.md) | Nenhum | Excluir um **objeto case.** |
| [Caso de fechamento](../api/ediscovery-case-close.md)        | Nenhum                                              | Feche um caso de Descoberta e. Para obter detalhes, consulte [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case). |
| [Caso De reabrir](../api/ediscovery-case-reopen.md)      | Nenhum                                              | Reabra um caso de Descoberta e Que foi fechado. Para obter detalhes, consulte [Reabrar um caso fechado](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).|
| Custodiantes |
| [Listar custodiantes](../api/ediscovery-case-list-custodians.md)   | [coleção microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) |Obter uma lista dos [objetos custodiantes](../resources/ediscovery-custodian.md) e suas propriedades.|
| [Criar custodiatário](../api/ediscovery-case-post-custodians.md)  | [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)           |Crie um novo [objeto custodiante.](../resources/ediscovery-custodian.md) Depois que o objeto custodiante for criado, você precisará criar o [usuário do custodianteSource](../resources/ediscovery-usersource.md) para fazer referência à caixa de correio e OneDrive for Business site.|
| Resções legais |
| [Listar legalHolds](../api/ediscovery-case-list-legalholds.md)   | [coleção microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) | Obter [os legalHolds](../resources/ediscovery-legalhold.md) que são aplicados a um caso.|
| [Criar legalHold](../api/ediscovery-case-post-legalholds.md)  | [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)           | Crie um novo [objeto legalHold.](../resources/ediscovery-legalhold.md)|
| Conjuntos de revisão |
| [Listar reviewSets](../api/ediscovery-case-list-reviewsets.md)   | [coleção microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Obter a lista de [reviewSets](../resources/ediscovery-reviewset.md) de um **objeto case.**|
| [Criar reviewSet](../api/ediscovery-case-post-reviewsets.md)  | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)           | Crie um novo [objeto reviewSet.](../resources/ediscovery-reviewset.md) O corpo da solicitação contém o nome de exibição do conjunto de revisão, que é a única propriedade writable.|
| Configurações de caso |
| [Obter caseSettings](../api/ediscovery-casesettings-get.md)|[microsoft.graph.ediscovery.caseSettings](../resources/ediscovery-casesettings.md)|Leia as propriedades e as relações de um [objeto microsoft.graph.ediscovery.caseSettings.](../resources/ediscovery-casesettings.md) |
| [Atualizar caseSettings](../api/ediscovery-casesettings-update.md)|[microsoft.graph.ediscovery.caseSsettings](../resources/ediscovery-casesettings.md)|Atualize as propriedades de [um objeto microsoft.graph.ediscovery.caseSettings.](../resources/ediscovery-casesettings.md) |
| [resetToDefault](../api/ediscovery-casesettings-resettodefault.md)|Nenhum|Redefinir todas as configurações para os valores padrão. |
| Coleções de origem |
| [Listar sourceCollections](../api/ediscovery-case-list-sourcecollections.md)|[coleção microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Obter a [sourceCollection](../resources/ediscovery-sourcecollection.md) de um **objeto case.**|
| [Criar sourceCollection](../api/ediscovery-case-post-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Crie um novo **objeto sourceCollection.**|
| Marcas |
| [Listar marcas](../api/ediscovery-case-list-tags.md)|[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Recupere uma lista de [objetos de](../resources/ediscovery-tag.md) marca de um caso de Descoberta Eletrônico.|
| [Criar marca](../api/ediscovery-case-post-tags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Crie uma nova marca para o caso especificado. As marcas são usadas em conjuntos de revisão durante a revisão do conteúdo.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|closedBy|[identitySet](/graph/api/resources/identityset)|O usuário que fechou a ocorrência.|
|closedDateTime|DateTimeOffset|A data e a hora em que o caso foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|createdBy|[identitySet](/graph/api/resources/identityset)|O usuário que criou o caso.|
|createdDateTime|DateTimeOffset|A data e a hora em que a entidade foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|description|Cadeia de caracteres|A descrição do caso.|
|displayName|Cadeia de caracteres|O nome do caso.|
|externalId|Cadeia de caracteres|O número de caso externo para referência do cliente.|
|id|Cadeia de caracteres| A ID do caso de Descoberta e. Somente leitura. |
|lastModifiedBy|[identitySet](/graph/api/resources/identityset)|O último usuário que modificou a entidade.|
|lastModifiedDateTime|DateTimeOffset| A data e a hora mais recentes em que o caso foi modificado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|status|microsoft.graph.ediscovery.caseStatus| O status do caso. Os valores possíveis `unknown` são , , , , e `active` `pendingDelete` `closing` `closed` `closedWithError` . Para obter detalhes, consulte a tabela a seguir.|

### <a name="casestatus-values"></a>valores caseStatus

|Member|Descrição|
|:----|-----------|
| desconhecido | O status do caso é desconhecido. |
| active | Case está ativo. |
| pendingDelete | O caso foi excluído, mas a exclusão não foi totalmente transatada. |
| closing | O caso foi fechado, mas a operação não foi totalmente transatada. |
| closed | O caso está fechado. |
| closedWithError | O caso está fechado, mas houve erros liberando ressarções no caso. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|custodiantes|[coleção microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)| Retorna uma lista de objetos **custodiantes** de caso para este **caso**.  Anulável.|
|legalHolds|[coleção microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)| Retorna uma lista de objetos **case legalHold** para este **caso**.  Anulável. |
|noncustodialDataSources|[coleção microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)| Retorna uma lista de objetos **case noncustodialDataSource** para este **caso**.  Anulável. |
|operations|[coleção microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md)| Retorna uma lista de objetos **de operação de** caso para este **caso**. Anulável. |
|reviewSets|[coleção microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)| Retorna uma lista de **objetos reviewSet** no caso. Somente leitura. Anulável. |
|caseSettings|[coleção microsoft.graph.ediscovery.caseSettings](../resources/ediscovery-casesettings.md)| Retorna uma lista **de objetos de configurações** no caso. Somente leitura. Anulável. |
|sourceCollections|[coleção microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Retorna uma lista de **objetos sourceCollection** associados a esse caso.|
|categorias|[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Retorna uma lista **de objetos de** marca associados a esse caso.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscovery.case"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.case",
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
  "description": "case resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
