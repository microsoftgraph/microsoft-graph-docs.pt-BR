---
title: Tipo de recurso resourceConnection
description: Representa conexões com recursos externos dos quais conexões mais especializadas serão derivadas.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: dd21fba95209dbcc1ce5f868b98fa818fe34b254
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856580"
---
# <a name="resourceconnection-resource-type"></a>Tipo de recurso resourceConnection

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa conexões com recursos externos dos quais conexões mais [especializadas, como operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) , serão derivadas.

Esse é um tipo abstrato.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar resourceConnections](../api/windowsupdates-updates-list-resourceconnections.md)|[Coleção microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md)|Obtenha uma lista dos [objetos resourceConnection](../resources/windowsupdates-resourceconnection.md) e suas propriedades.|
|[Obter resourceConnection](../api/windowsupdates-resourceconnection-get.md)|[microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md)|Leia as propriedades e as relações de um [objeto resourceConnection](../resources/windowsupdates-resourceconnection.md) .|
|[Excluir resourceConnection](../api/windowsupdates-resourceconnection-delete.md)|Nenhum|Exclua [um objeto resourceConnection](../resources/windowsupdates-resourceconnection.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Um identificador para a conexão de recurso. Chave. Não anulável. Somente leitura. Devolvido por padrão.|
|state|microsoft.graph.windowsUpdates.resourceConnectionState|O estado da conexão. Os valores possíveis são: `connected`, `notAuthorized`, `notFound`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.resourceConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.resourceConnection",
  "id": "String (identifier)",
  "state": "String"
}
```

