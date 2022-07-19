---
title: Tipo de recurso operationalInsightsConnection
description: Representa um resourceConnection especializado que vincula um workspace do Log Analytics ao serviço de implantação Windows Update para Empresas.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 07725da7d19cdf4c7fdb232f45823e75ffe37d2d
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856581"
---
# <a name="operationalinsightsconnection-resource-type"></a>Tipo de recurso operationalInsightsConnection

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um [resourceConnection especializado que](../resources/windowsupdates-resourceconnection.md) vincula um workspace do Log Analytics ao serviço de implantação Windows Update para Empresas.

Herda de [resourceConnection](../resources/windowsupdates-resourceconnection.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar operationalInsightsConnections](../api/windowsupdates-updates-list-resourceconnections-operationalinsightsconnection.md)|[coleção microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md)|Obtenha uma lista dos [objetos operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) e suas propriedades.|
|[Criar operationalInsightsConnection](../api/windowsupdates-updates-post-resourceconnections-operationalinsightsconnection.md)|[microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md)|Crie um novo [objeto operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .|
|[Obter operationalInsightsConnection](../api/windowsupdates-operationalinsightsconnection-get.md)|[microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md)|Leia as propriedades e as relações de um [objeto operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .|
|[Excluir operationalInsightsConnection](../api/windowsupdates-operationalinsightsconnection-delete.md)|Nenhum|[Exclua um objeto operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|azureResourceGroupName|Cadeia de caracteres|O nome do grupo de recursos do Azure que contém o workspace do Log Analytics.|
|azureSubscriptionId|String|A ID da assinatura do Azure que contém o workspace do Log Analytics.|
|id|Cadeia de caracteres|Um identificador para a conexão de recurso. Chave. Não anulável. Somente leitura. Devolvido por padrão.|
|state|microsoft.graph.windowsUpdates.resourceConnectionState|O estado da conexão. Os valores possíveis são: `connected`, `notAuthorized`, `notFound`, `unknownFutureValue`.|
|Workspacename|Cadeia de caracteres|O nome do workspace do Log Analytics.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "baseType": "microsoft.graph.windowsUpdates.resourceConnection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "azureResourceGroupName": "String",  
  "azureSubscriptionId": "String",
  "id": "String (identifier)",
  "state": "String",
  "workspaceName": "String"
}
```

