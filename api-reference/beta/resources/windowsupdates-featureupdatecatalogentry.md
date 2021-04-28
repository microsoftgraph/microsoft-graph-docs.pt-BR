---
title: tipo de recurso featureUpdateCatalogEntry
description: Metadados para uma atualização Windows 10 de recursos que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 64ad4c2506a2d8f90276e50e7fe5288e1af1d8db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067251"
---
# <a name="featureupdatecatalogentry-resource-type"></a>tipo de recurso featureUpdateCatalogEntry

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Metadados para uma atualização Windows 10 de recursos que você pode aprovar para implantação.

Windows 10 de recursos são lançadas anualmente e contêm novos recursos para Windows 10. Instalar essas atualizações aumenta o número Windows 10 de com build e normalmente resulta em um novo ciclo de vida de manutenção e data de término do serviço. A Microsoft recomenda que as organizações implantem regularmente novas atualizações de recursos como parte da adoção Windows como um serviço.

Herda de [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|A data em que o conteúdo não está mais disponível para implantação usando o serviço. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|displayName|Cadeia de caracteres|O nome de exibição do conteúdo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|id|Cadeia de caracteres|O identificador exclusivo para a entrada do catálogo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
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

