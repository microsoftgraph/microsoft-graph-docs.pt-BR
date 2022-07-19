---
title: Tipo de recurso ediscoveryCase
description: No contexto da Descoberta Eletrônica, contém custodiantes, retenções, coleções e conjuntos de revisão.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 3348c6c718a1ccd23977b4b1164cc21111198eac
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839220"
---
# <a name="ediscoverycase-resource-type"></a>Tipo de recurso ediscoveryCase

Namespace: microsoft.graph.security



No contexto da Descoberta Eletrônica, contém custodiantes, pesquisas, conjuntos de revisão. Para obter detalhes, [consulte Visão geral Descoberta Eletrônica do Microsoft Purview (Premium)](/microsoft-365/compliance/overview-ediscovery-20).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryCases](../api/security-casesroot-list-ediscoverycases.md)|[coleção microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|Obtenha uma lista dos [objetos ediscoveryCase](../resources/security-ediscoverycase.md) e suas propriedades.|
|[Criar ediscoveryCase](../api/security-casesroot-post-ediscoverycases.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|Crie um novo [objeto ediscoveryCase](../resources/security-ediscoverycase.md) .|
|[Obter ediscoveryCase](../api/security-ediscoverycase-get.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|Leia as propriedades e as relações de [um objeto ediscoveryCase](../resources/security-ediscoverycase.md) .|
|[Atualizar ediscoveryCase](../api/security-ediscoverycase-update.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|Atualize as propriedades de [um objeto ediscoveryCase](../resources/security-ediscoverycase.md) .|
|[Excluir ediscoveryCase](../api/security-casesroot-delete-ediscoverycases.md)|Nenhum|[Exclua um objeto ediscoveryCase](../resources/security-ediscoverycase.md).|
|[Listar custodiantes](../api/security-ediscoverycase-list-custodians.md)|[coleção microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Obtenha os recursos de ediscoveryCustodian da propriedade de navegação dos custodiantes.|
|[Criar ediscoveryCustodian](../api/security-ediscoverycase-post-custodians.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Crie um novo objeto ediscoveryCustodian.|
|[Listar noncustodialDataSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[coleção microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Obtenha os recursos de ediscoveryNoncustodialDataSource da propriedade de navegação nãocustodialDataSources.|
|[Criar ediscoveryNoncustodialDataSource](../api/security-ediscoverycase-post-noncustodialdatasources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Crie um novo objeto ediscoveryNoncustodialDataSource.|
|[Listar operações](../api/security-ediscoverycase-list-operations.md)|[coleção microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|Obtenha os recursos caseOperation da propriedade de navegação de operações.|
|[Listar reviewSets](../api/security-ediscoverycase-list-reviewsets.md)|[coleção microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Obtenha os recursos ediscoveryReviewSet da propriedade de navegação reviewSets.|
|[Criar ediscoveryReviewSet](../api/security-ediscoverycase-post-reviewsets.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Crie um novo objeto ediscoveryReviewSet.|
|[Listar pesquisas](../api/security-ediscoverycase-list-searches.md)|[coleção microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Obtenha os recursos de ediscoverySearch da propriedade de navegação de pesquisas.|
|[Criar ediscoverySearch](../api/security-ediscoverycase-post-searches.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Crie um novo objeto ediscoverySearch.|
|[Listar marcas](../api/security-ediscoverycase-list-tags.md)|[coleção microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Obtenha os recursos ediscoveryReviewTag da propriedade de navegação de marcas.|
|[Criar ediscoveryReviewTag](../api/security-ediscoverycase-post-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Crie um novo objeto ediscoveryReviewTag.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|closedBy|[microsoft.graph.identitySet](../resources/identityset.md)|O usuário que fechou o caso.|
|closedDateTime|DateTimeOffset|A data e a hora em que o caso foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|O usuário que criou o caso.|
|createdDateTime|DateTimeOffset|A data e a hora em que a entidade foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|descrição|String|A descrição do caso.|
|displayName|String|O nome do caso.|
|externalId|Cadeia de caracteres|O número de caso externo para referência de cliente.|
|id|String|A ID do caso de Descoberta Eletrônica. Somente leitura. |
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|O último usuário que modificou o caso.
|lastModifiedDateTime|DateTimeOffset|A data e a hora mais recentes em que o caso foi modificado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|status|microsoft.graph.security.caseStatus|O status do caso. Os valores possíveis `unknown`são , `active``pendingDelete`, `closing`, `closed`e `closedWithError`. Para obter detalhes, consulte a tabela a seguir.

### <a name="casestatus-values"></a>valores caseStatus

|Member|Descrição|
|:----|-----------|
| desconhecido | O status do caso é desconhecido. |
| Ativo | O caso está ativo. |
| pendingDelete | O caso foi excluído, mas a exclusão não foi totalmente transacionada. |
| Fechar | O caso foi fechado, mas a operação não foi totalmente transacionada. |
| Fechado | O caso está fechado. |
| closedWithError | O caso está fechado, mas houve erros ao liberar retenções no caso. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Guardiões|[coleção microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Retorna uma lista de objetos **case ediscoveryCustodian** para esse **caso**.|
|noncustodialDataSources|[coleção microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Retorna uma lista de objetos **case ediscoveryNoncustodialDataSource** para esse **caso**.|
|operations|[coleção microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|Retorna uma lista de objetos **caseOperation** case para esse **caso**.|
|reviewSets|[coleção microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Retorna uma lista de **objetos eDiscoveryReviewSet** no caso.|
|Pesquisas|[coleção microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Retorna uma lista de **objetos eDiscoverySearch** associados a esse caso.|
|settings|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|Retorna uma lista de **objetos eDIscoverySettings** no caso.|
|tags|[coleção microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Retorna uma lista de **objetos ediscoveryReviewTag** associados a esse caso.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCase",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String"
}
```

