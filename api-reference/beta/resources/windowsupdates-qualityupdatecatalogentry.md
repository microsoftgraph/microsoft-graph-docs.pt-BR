---
title: Tipo de recurso qualityUpdateCatalogEntry
description: Metadados para uma atualização Windows 10 de qualidade que você pode aprovar para implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: bdac770931e6986ac4233bf32d0eb82bc9a08be4
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863009"
---
# <a name="qualityupdatecatalogentry-resource-type"></a>Tipo de recurso qualityUpdateCatalogEntry

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Metadados para uma atualização Windows 10 de qualidade que você pode aprovar para implantação.

Windows 10 de qualidade são lançadas uma ou mais vezes por mês. Essas atualizações contêm correções de segurança e qualidade e geralmente são lançadas na segunda terça-feira de cada mês, embora possam ser lançadas a qualquer momento. Essas atualizações são cumulativas, portanto, as versões posteriores sempre contêm todas as correções anteriores. A Microsoft recomenda manter os dispositivos atualizados instalando as atualizações de qualidade mais recentes assim que elas estão disponíveis. 

Herda de [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|A data em que o conteúdo não está mais disponível para implantação usando o serviço. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|displayName|String|O nome de exibição do conteúdo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|id|String|O identificador exclusivo para a entrada do catálogo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|isExpeditable|Booliano|Indica se o conteúdo pode ser implantado como uma atualização de qualidade acelerada. Somente leitura.|
|qualityUpdateClassification|microsoft.graph.windowsUpdates.qualityUpdateClassification|A classificação na atualização de qualidade. Os valores possíveis são: `all`, `security`, `nonSecurity`, `unknownFutureValue`. Somente leitura.|
|releaseDateTime|DateTimeOffset|A data de lançamento do conteúdo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "isExpeditable": "Boolean",
  "qualityUpdateClassification": "String"
}
```

