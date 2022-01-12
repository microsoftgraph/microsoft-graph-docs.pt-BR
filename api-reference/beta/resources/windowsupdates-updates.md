---
title: atualiza tipo de recurso
description: Entidade que atua como um contêiner para todas as Windows de implantação do Update for Business.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 748ef5c6e8e334b2e1c311c07617c181490f4f39
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861537"
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

