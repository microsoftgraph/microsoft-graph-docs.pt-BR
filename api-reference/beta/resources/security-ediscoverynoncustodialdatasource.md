---
title: Tipo de recurso ediscoveryNoncustodialDataSource
description: As fontes de dados não custodiais permitem que você adicione dados a um caso sem precisar associá-los a um guardião.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: fcf2022747ee7b98526d522eecc268be2def490d
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945040"
---
# <a name="ediscoverynoncustodialdatasource-resource-type"></a>Tipo de recurso ediscoveryNoncustodialDataSource

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fontes de dados não custodiais permitem que você adicione dados a um caso sem precisar associá-los a um guardião. Para saber mais, visite [Adicionar fontes de dados não custodiais a um caso de Descoberta Eletrônica Avançada ](/microsoft-365/compliance/non-custodial-data-sources)


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
|[Listar ediscoveryIndexOperation](../api/security-ediscoverycustodian-list-lastindexoperation.md)|[coleção microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Obtenha os recursos de ediscoveryIndexOperation da propriedade de navegação lastIndexOperation.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora criadas do nonCustodialDataSource. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|displayName|Cadeia de caracteres|Nome de exibição do noncustodialDataSource. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|id|String|Identificador exclusivo do nonCustodialDataSource. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do nonCustodialDataSource. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|releasedDateTime|DateTimeOffset|Data e hora em que o nonCustodialDataSource foi liberado do caso. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|status|Cadeia de caracteres|Status mais recente do nonCustodialDataSource. Herdado [de microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md). Os valores possíveis são: `Active` e `Released`.|
|holdStatus|Cadeia de caracteres|O status de retenção do nonCustodialDataSource.Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|

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