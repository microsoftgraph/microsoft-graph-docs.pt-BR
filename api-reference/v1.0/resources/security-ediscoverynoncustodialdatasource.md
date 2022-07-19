---
title: Tipo de recurso ediscoveryNoncustodialDataSource
description: As fontes de dados não custodiais permitem que você adicione dados a um caso sem precisar associá-los a um guardião.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 12b01d84aa5ce9642cc227bc192cb078f1484793
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839061"
---
# <a name="ediscoverynoncustodialdatasource-resource-type"></a>Tipo de recurso ediscoveryNoncustodialDataSource

Namespace: microsoft.graph.security



Permite a adição de dados a um caso de Descoberta Eletrônica sem associá-los a um guardião. Para obter detalhes, [consulte Adicionar fontes de dados não custodiais a um caso de Descoberta Eletrônica (Premium](/microsoft-365/compliance/non-custodial-data-sources)).


Herda de [dataSourceContainer](../resources/security-datasourcecontainer.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar ediscoveryNoncustodialDataSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[coleção microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Obtenha uma lista dos [objetos ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) e suas propriedades.|
|[Criar ediscoveryNoncustodialDataSource](../api/security-ediscoverysearch-post-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Crie um novo [objeto ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .|
|[Obter ediscoveryNoncustodialDataSource](../api/security-ediscoverynoncustodialdatasource-get.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Leia as propriedades e as relações de um [objeto ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .|
|[updateIndex](../api/security-ediscoverynoncustodialdatasource-updateindex.md)|Nenhum|Dispara uma indexOperation para tornar uma fonte de dados não custodiante e fontes de dados associadas pesquisáveis.|
|[Lançamento](../api/security-ediscoverynoncustodialdatasource-release.md)|Nenhum|Libere uma fonte de dados não custodiante de um caso.|
|[applyHold](../api/security-ediscoverynoncustodialdatasource-applyhold.md)|Nenhum|Inicie o processo de aplicação de retenção a fontes de dados não custodiais da Descoberta Eletrônica.|
|[removeHold](../api/security-ediscoverynoncustodialdatasource-removehold.md)|Nenhum|Inicie o processo de remoção da retenção de fontes de dados não custodiais da Descoberta Eletrônica.|
|[Listar ediscoveryIndexOperation](../api/security-ediscoverycustodian-list-lastindexoperation.md)|[coleção microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Obtenha uma lista da [ediscoveryIndexOperation associada](../resources/security-ediscoveryindexoperation.md) a [um ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora criadas do nonCustodialDataSource. Herdado [de microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md).|
|displayName|String|Nome de exibição do noncustodialDataSource. Herdado [de microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md).|
|id|String|Identificador exclusivo do nonCustodialDataSource. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do nonCustodialDataSource. Herdado [de microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md).|
|releasedDateTime|DateTimeOffset|Data e hora em que o nonCustodialDataSource foi liberado do caso. Herdado [de microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md).|
|status|microsoft.graph.security.dataSourceContainerStatus|Status mais recente do nonCustodialDataSource. Herdado [de microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md). Os valores possíveis são: `Active` e `Released`.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|O status de retenção do nonCustodialDataSource.Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Datasource|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|Fonte de usuário ou fonte de dados do site do SharePoint como fonte de dados não custodiante.|
|lastIndexOperation|[microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Entidade de operação que representa a indexação mais recente para a fonte de dados não custodiante.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryNoncustodialDataSource",
  "baseType": "microsoft.graph.security.dataSourceContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryNoncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
