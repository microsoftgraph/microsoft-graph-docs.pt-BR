---
title: tipo de recurso updates
description: Entidade que atua como um contêiner para todas as Windows Update do serviço de implantação para Empresas.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a315516e8ded53cfacbe94c0ace2d9c12c5b3f78
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856411"
---
# <a name="updates-resource-type"></a>tipo de recurso updates

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade que atua como um contêiner para todas as Windows Update do serviço de implantação para Empresas.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Somente leitura. Herdado da [entidade](../resources/entity.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Catálogo|[microsoft.graph.windowsUpdates.catalog](../resources/windowsupdates-catalog.md)|Catálogo de conteúdo que pode ser aprovado para implantação pelo serviço de implantação. Somente leitura.|
|Implantações|[Coleção microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Implantações criadas usando o serviço de implantação. Somente leitura.|
|resourceConnections|[Coleção microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md)|Conexões de serviço com recursos externos, como workspaces de análise.|
|updatableAssets|[Coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Ativos registrados com o serviço de implantação que podem receber atualizações. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updates",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updates",
  "id": "String (identifier)"
}
```

