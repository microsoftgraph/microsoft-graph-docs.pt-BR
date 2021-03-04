---
title: Tipo de recurso sourceCollection
description: Representa uma coleção eDiscovery, comumente conhecida como pesquisa.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 86ecf3adb64be2b216fdc167b29c10a850e25af6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445895"
---
# <a name="sourcecollection-resource-type"></a>Tipo de recurso sourceCollection

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção eDiscovery, comumente conhecida como pesquisa. Para obter detalhes, [consulte Coletar dados para uma ocorrência em Descoberta Avançada de eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sourceCollections](../api/ediscovery-case-list-sourcecollections.md)|[coleção microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Obter uma lista dos **objetos sourceCollection** e suas propriedades.|
|[Criar sourceCollection](../api/ediscovery-case-post-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Crie um novo **objeto sourceCollection.**|
|[Obter sourceCollection](../api/ediscovery-sourcecollection-get.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Leia as propriedades e as relações de um **objeto sourceCollection.**|
|[Atualizar sourceCollection](../api/ediscovery-sourcecollection-update.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Atualize as propriedades de um **objeto sourceCollection.**|
|[Excluir sourceCollection](../api/ediscovery-sourcecollection-delete.md)|Nenhum(a)|Exclua **um objeto sourceCollection.**|
|[estimateStatistics](../api/ediscovery-sourcecollection-estimatestatistics.md)|Nenhum(a)|Execute uma estimativa do número de emails e documentos na coleção de origem.|
|[Listar additionalSources](../api/ediscovery-sourcecollection-list-additionalsources.md)|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Obter uma lista de **objetos dataSource adicionais** associados a uma coleção de origem.|
|[Listar custodiadoresSources](../api/ediscovery-sourcecollection-list-custodiansources.md)|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Obter uma lista de **objetos dataSource adicionais** associados a uma coleção de origem.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentQuery|String|A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language). Para obter detalhes, consulte [Consultas de palavra-chave e condições de pesquisa para Pesquisa de Conteúdo e Descoberta De Conteúdo.](https://docs.microsoft.com/microsoft-365/compliance/keyword-queries-and-search-conditions)  Você pode refinar pesquisas usando campos emparelhados com valores; por exemplo, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o sourceCollection**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que o sourceCollection** foi criado.|
|descrição|String|A descrição da **sourceCollection**|
|displayName|String|O nome de exibição da **sourceCollection**|
|id|String| A ID da **sourceCollection**. Somente leitura. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|O último usuário que modificou **o sourceCollection**.|
|lastModifiedDateTime|DateTimeOffset|A última data e hora em **que o sourceCollection** foi modificado.|
|tenantSources|microsoft.graph.ediscovery.tenantSources|Quando especificado, a coleção se estenderá por um serviço para uma carga de trabalho inteira. Os valores possíveis são: `allMailboxes` e `allSites`.|

### <a name="tenantsources-values"></a>valores tenantSources

|Member|Descrição|
|:----|-----------|
|allMailboxes| Inclua todas as caixas de correio na coleção. |
|allSites| Inclua todos os sites na coleção. |

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|additionalSources|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Adiciona uma fonte adicional à **sourceCollection**.|
|addToReviewSetOperation|[microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md)|Adiciona os resultados do **sourceCollection** ao **reviewSet especificado.**|
|custodianSources|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|**Fontes de** custodia que estão incluídas na **sourceCollection**.|
|lastEstimateStatisticsOperation|[microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)|A última operação de estimativa associada à **sourceCollection**.|

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
  "tenantSources": "String"
}
```
