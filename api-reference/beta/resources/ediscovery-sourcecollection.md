---
title: Tipo de recurso sourceCollection
description: Representa uma coleção eDiscovery, comumente conhecida como pesquisa.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a67599c4a813e1ac7e354d1fd2b0c26c8eb366bb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101883"
---
# <a name="sourcecollection-resource-type"></a>Tipo de recurso sourceCollection

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção eDiscovery, comumente conhecida como pesquisa. Para detalhes, consulte [Coletar dados para um caso na Descoberta Eletrônica Avançada](/microsoft-365/compliance/collecting-data-for-ediscovery).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Adicionar additionalSource](../api/ediscovery-sourcecollection-post-additionalsources.md)|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Adicione um **objeto dataSource** adicional à coleção de origem.|
|[Adicionar custodianSource](../api/ediscovery-sourcecollection-post-custodiansources.md)|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Adicionar um objeto **dataSource custodiante** à coleção de origem.|
|[Adicionar noncustodialSource](../api/ediscovery-sourcecollection-post-noncustodialsources.md)|[coleção microsoft.graph.ediscovery.noncustodialSource](../resources/ediscovery-noncustodialdatasource.md)|Adicione um objeto **noncustodialSource** de origem não custodial à coleção de origem.|
|[Listar sourceCollections](../api/ediscovery-case-list-sourcecollections.md)|[coleção microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Obter uma lista dos **objetos sourceCollection** e suas propriedades.|
|[Criar sourceCollection](../api/ediscovery-case-post-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Crie um novo **objeto sourceCollection.**|
|[Obter sourceCollection](../api/ediscovery-sourcecollection-get.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Leia as propriedades e as relações de um **objeto sourceCollection.**|
|[Atualizar sourceCollection](../api/ediscovery-sourcecollection-update.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Atualize as propriedades de um **objeto sourceCollection.**|
|[Excluir sourceCollection](../api/ediscovery-sourcecollection-delete.md)|Nenhum|Exclua **um objeto sourceCollection.**|
|[estimateStatistics](../api/ediscovery-sourcecollection-estimatestatistics.md)|Nenhum|Execute uma estimativa do número de emails e documentos na coleção de origem.|
|[Listar additionalSources](../api/ediscovery-sourcecollection-list-additionalsources.md)|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Obter uma lista de **objetos dataSource adicionais** associados a uma coleção de origem.|
|[Listar custodiadoresSources](../api/ediscovery-sourcecollection-list-custodiansources.md)|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Obter uma lista de objetos **dataSource custodiantes** associados a uma coleção de origem.|
|[Listar noncustodialSources](../api/ediscovery-sourcecollection-list-noncustodialsources.md)|[coleção microsoft.graph.ediscovery.noncustodialSource](../resources/ediscovery-noncustodialdatasource.md)|Obter uma lista de fontes não custodiais **objetos noncustodialSource** associados a uma coleção de origem.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentQuery|Cadeia de caracteres|A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language). Para obter detalhes, consulte [Consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta De Conteúdo.](/microsoft-365/compliance/keyword-queries-and-search-conditions) Você pode refinar pesquisas usando campos emparelhados com valores; por exemplo, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*.|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o sourceCollection**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que o sourceCollection** foi criado.|
|dataSourceScopes|microsoft.graph.ediscovery.dataSourceScopes|Quando especificado, a coleção se estenderá por um serviço para uma carga de trabalho inteira. Os valores possíveis são: `none`, `allTenantMailboxes`, `allTenantSites`, `allCaseCustodians`, `allCaseNoncustodialDataSources`.|
|description|Cadeia de caracteres|A descrição da **sourceCollection**.|
|displayName|Cadeia de caracteres|O nome de exibição do **sourceCollection**.|
|id|Cadeia de caracteres| A ID da **sourceCollection**. Somente leitura. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|O último usuário que modificou **o sourceCollection**.|
|lastModifiedDateTime|DateTimeOffset|A última data e hora em **que o sourceCollection** foi modificado.|

### <a name="datasourcescopes-values"></a>valores dataSourceScopes

|Member|Descrição|
|:----|-----------|
|none|Não especifique nenhum escopo - os locais seriam referenciados separadamente.|
|allTenantMailboxes|Inclua todas as caixas de correio de locatários **na sourceCollection**.|
|allTenantSites|Inclua todos os sites de **locatários no sourceCollection**.|
|allCaseCustodians|Inclua todos os locais de custodia na **sourceCollection**.|
|allCaseNoncustodialDataSources|Inclua todas as fontes de dados não custodiais na **sourceCollection**.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|additionalSources|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Adiciona uma fonte adicional à **sourceCollection**.|
|addToReviewSetOperation|[microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md)|Adiciona os resultados do **sourceCollection** ao **reviewSet especificado.**|
|custodianSources|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|**Fontes de** custodia que estão incluídas na **sourceCollection**.|
|lastEstimateStatisticsOperation|[microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)|A última operação de estimativa associada à **sourceCollection**.|
|noncustodialSources|[coleção microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|**fontes noncustodialDataSource** incluídas na **sourceCollection**|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.sourceCollection",
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