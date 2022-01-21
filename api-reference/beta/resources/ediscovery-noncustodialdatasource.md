---
title: Tipo de recurso noncustodialDataSource
description: Fontes de dados não custodiais permitem adicionar dados a um caso sem precisar associá-los a um custodiante
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 238a09015efa5f445dcc92390ee7a8eff19d8df5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115187"
---
# <a name="noncustodialdatasource-resource-type"></a>Tipo de recurso noncustodialDataSource

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fontes de dados não custodiais permitem adicionar dados a um caso sem precisar associá-los a um custodiante. Para saber mais, visite Adicionar fontes de dados não [custodiais a um Advanced eDiscovery caso](/microsoft-365/compliance/non-custodial-data-sources)

Herda de [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar noncustodialDataSources](../api/ediscovery-noncustodialdatasource-list.md)|[coleção microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|Obter uma lista dos [objetos noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) e suas propriedades.|
|[Obter noncustodialDataSource](../api/ediscovery-noncustodialdatasource-get.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|Leia as propriedades e as relações de [um objeto noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)|
|[Liberar dadosSource](../api/ediscovery-noncustodialdatasource-release.md)|Nenhum|Libera uma fonte de dados não custodiada.|
|[Listar dadosSource](../api/ediscovery-noncustodialdatasource-list-datasource.md)|[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Obter os recursos dataSource da propriedade de navegação dataSource.|
|[Criar dataSource](../api/ediscovery-noncustodialdatasource-post.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Crie um novo objeto dataSource.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applyHoldToSource|Booliano|Indica se a espera é aplicada à fonte de dados não custodial (como caixa de correio ou site).|
|createdDateTime|DateTimeOffset|Data e hora criadas do nonCustodialDataSource. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|displayName|Cadeia de caracteres|Nome de exibição do noncustodialDataSource. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|id|Cadeia de caracteres|Identificador exclusivo do nonCustodialDataSource. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do nonCustodialDataSource. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|releasedDateTime|DateTimeOffset|Data e hora em que o nonCustodialDataSource foi liberado do caso. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|status|microsoft.graph.ediscovery.dataSourceContainerStatus|Status mais recente do nonCustodialDataSource. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md). Os valores possíveis são: `Active`, `Released`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|dataSource|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Fonte de usuário ou SharePoint de dados do site como fonte de dados não custodiada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource",
  "baseType": "microsoft.graph.ediscovery.dataSourceContainer",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.noncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "applyHoldToSource": "Boolean"
}
```