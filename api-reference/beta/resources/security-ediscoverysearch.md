---
title: Tipo de recurso ediscoverySearch
description: Representa uma pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ccff50d8654bbd6723ae21df4163b80afc310ead
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837356"
---
# <a name="ediscoverysearch-resource-type"></a>Tipo de recurso ediscoverySearch

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma pesquisa de Descoberta Eletrônica. Para obter detalhes, [consulte Coletar dados para um caso na Descoberta Eletrônica (Premium)](/microsoft-365/compliance/collecting-data-for-ediscovery).


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoverySearches](../api/security-ediscoverycase-list-searches.md)|[coleção microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Obtenha uma lista dos [objetos ediscoverySearch](../resources/security-ediscoverysearch.md) e suas propriedades.|
|[Criar ediscoverySearch](../api/security-ediscoverycase-post-searches.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Crie um novo [objeto ediscoverySearch](../resources/security-ediscoverysearch.md) .|
|[Obter descoberta eletrônicaSearch](../api/security-ediscoverysearch-get.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Leia as propriedades e as relações de [um objeto ediscoverySearch](../resources/security-ediscoverysearch.md) .|
|[Atualizar ediscoverySearch](../api/security-ediscoverysearch-update.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Atualize as propriedades de [um objeto ediscoverySearch](../resources/security-ediscoverysearch.md) .|
|[Excluir ediscoverySearch](../api/security-ediscoverycase-delete-searches.md)|Nenhum|[Exclua um objeto microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md).|
|[estimateStatistics](../api/security-ediscoverysearch-estimatestatistics.md)|Nenhum|Execute uma operação de estimativa de estatísticas nos dados contidos na pesquisa de Descoberta Eletrônica.|
|[purgeData](../api/security-ediscoverysearch-purgedata.md)|Nenhum|Execute uma operação de limpeza de dados nos dados do Teams contidos na pesquisa de Descoberta Eletrônica.|
|[Listar additionalSources](../api/security-ediscoverysearch-list-additionalsources.md)|[Coleção microsoft.graph.security.dataSource](../resources/security-datasource.md)|Obtenha a lista de [fontes adicionais](../resources/security-datasource.md) associadas a [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).|
|[Adicionar additionalSources](../api/security-ediscoverysearch-post-additionalsources.md)|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|Crie uma nova [fonte adicional](../resources/security-datasource.md) associada a [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).|
|[Listar ediscoveryEstimateOperation](../api/security-ediscoverysearch-list-lastestimatestatisticsoperation.md)|[coleção microsoft.graph.security.ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md)|Obtenha os últimos [objetos ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md) e suas propriedades.|
|[Listar custodianSources](../api/security-ediscoverysearch-list-custodiansources.md)|[Coleção microsoft.graph.security.dataSource](../resources/security-datasource.md)|Obtenha a lista de fontes de dados de custódia associadas a [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).|
|[Adicionar custodianSources](../api/security-ediscoverysearch-post-custodiansources.md)|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|Crie uma nova fonte custodiante associada a [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).|
|[Remover custodianSources](../api/security-ediscoverysearch-delete-custodiansources.md)|Nenhum|Remova um [objeto microsoft.graph.security.dataSource](../resources/security-datasource.md) .|
|[Listar noncustodialSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[coleção microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Obtenha a lista de não custodiaisSources associados a uma [pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).|
|[Adicionar noncustodialSources](../api/security-ediscoverysearch-post-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Crie uma nova fonte não custodiante associada a [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).|
|[Remover noncustodialSources](../api/security-ediscoverysearch-delete-noncustodialsources.md)|Nenhum|Remova um [objeto microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentQuery|Cadeia de caracteres|A cadeia de caracteres de consulta na consulta KQL (Linguagem de Consulta de Palavra-chave). Para obter detalhes, consulte [consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta Eletrônica](/microsoft-365/compliance/keyword-queries-and-search-conditions). Você pode refinar pesquisas usando campos emparelhados com valores; por exemplo, assunto:"Finanças Trimestrais *" E Data>=01/06/2016 E Data<=01/07/2016*.|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **a pesquisa de Descoberta Eletrônica**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que a pesquisa de Descoberta** Eletrônica foi criada.|
|dataSourceScopes|microsoft.graph.security.dataSourceScopes|Quando especificado, a coleção abrangerá um serviço para uma carga de trabalho inteira. Os valores possíveis são: `none`, `allTenantMailboxes`, `allTenantSites`, `allCaseCustodians`, `allCaseNoncustodialDataSources`.|
|descrição|Cadeia de caracteres|A descrição da **pesquisa de Descoberta Eletrônica**.|
|displayName|String|O nome de exibição da **pesquisa de Descoberta Eletrônica**.|
|id|String| A ID da **pesquisa de Descoberta Eletrônica**. Somente leitura. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|O último usuário que modificou **a pesquisa de Descoberta Eletrônica**.|
|lastModifiedDateTime|DateTimeOffset|A última data e hora em que **a pesquisa de Descoberta Eletrônica** foi modificada.|

### <a name="datasourcescopes-values"></a>Valores de dataSourceScopes

|Member|Descrição|
|:----|-----------|
|none|Não especifique nenhum escopo - os locais seriam referenciados separadamente.|
|allTenantMailboxes|Inclua todas as caixas de correio de locatário na **pesquisa de Descoberta Eletrônica**.|
|allTenantSites|Inclua todos os sites de locatário **na pesquisa de Descoberta Eletrônica**.|
|allCaseCustodians|Inclua todos os locais de custodiante na **pesquisa de Descoberta Eletrônica**.|
|allCaseNoncustodialDataSources|Inclua todas as fontes de dados não custodiais na **pesquisa de Descoberta Eletrônica**.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|additionalSources|[Coleção microsoft.graph.security.dataSource](../resources/security-datasource.md)|Adiciona uma fonte adicional à **pesquisa de Descoberta Eletrônica**.|
|addToReviewSetOperation|[microsoft.graph.security.ediscoveryAddToReviewSetOperation](../resources/security-ediscoveryaddtoreviewsetoperation.md)|Adiciona os resultados da **pesquisa de Descoberta Eletrônica** ao **reviewSet especificado**.|
|custodianSources|[Coleção microsoft.graph.security.dataSource](../resources/security-datasource.md)|**Fontes custodiante** incluídas na **pesquisa de Descoberta Eletrônica**.|
|lastEstimateStatisticsOperation|[microsoft.graph.security.ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md)|A última operação de estimativa associada à **pesquisa de Descoberta Eletrônica**.|
|noncustodialSources|[coleção microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|**fontes noncustodialDataSource** incluídas na **pesquisa de Descoberta Eletrônica**|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoverySearch",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoverySearch",
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
  "contentQuery": "String",
  "dataSourceScopes": "String"
}
```