---
title: atualiza tipo de recurso
description: Entidade que atua como um contêiner para todas as Windows de implantação do Update for Business.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0306dbadd815bdd8ff0ffde5719a950bcdff4683
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067228"
---
# <a name="updates-resource-type"></a>atualiza tipo de recurso

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade que atua como um contêiner para todas as Windows de implantação do Update for Business.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Somente leitura. Herdado da [entidade](../resources/entity.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|catalog|[microsoft.graph.windowsUpdates.catalog](../resources/windowsupdates-catalog.md)|Catálogo de conteúdo que pode ser aprovado para implantação pelo serviço de implantação. Somente leitura.|
|implantações|[coleção microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Implantações criadas usando o serviço de implantação. Somente leitura.|
|updatableAssets|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Ativos registrados no serviço de implantação que podem receber atualizações. Somente leitura.|

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

