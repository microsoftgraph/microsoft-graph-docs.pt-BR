---
title: tipo de recurso featureUpdateCatalogEntry
description: Metadados para uma atualização Windows 10 de recursos que você pode aprovar para implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 94403127fdbc8c263df546c2dfd1359c87894a06
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861638"
---
# <a name="featureupdatecatalogentry-resource-type"></a>tipo de recurso featureUpdateCatalogEntry

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Metadados para uma atualização Windows 10 de recursos que você pode aprovar para implantação.

Windows 10 de recursos são lançadas anualmente e contêm novos recursos para Windows 10. Instalar essas atualizações aumenta o número Windows 10 de com build e normalmente resulta em um novo ciclo de vida de manutenção e data de término do serviço. A Microsoft recomenda que as organizações implantem regularmente novas atualizações de recursos como parte da adoção Windows como serviço.

Herda de [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|A data em que o conteúdo não está mais disponível para implantação usando o serviço. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|displayName|String|O nome de exibição do conteúdo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|id|String|O identificador exclusivo para a entrada do catálogo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|releaseDateTime|DateTimeOffset|A data de lançamento do conteúdo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|versão|String|A versão da atualização de recursos. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "version": "String"
}
```

