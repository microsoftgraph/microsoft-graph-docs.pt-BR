---
title: Tipo de recurso qualityUpdateCatalogEntry
description: Metadados para uma atualização Windows 10 de qualidade que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f455919bfc3d5f0e6c4e2aa5ef6a6b630b66bc52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067791"
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
|displayName|Cadeia de caracteres|O nome de exibição do conteúdo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|id|Cadeia de caracteres|O identificador exclusivo para a entrada do catálogo. Somente leitura. Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|isExpeditable|Boolean|Indica se o conteúdo pode ser implantado como uma atualização de qualidade acelerada. Somente leitura.|
|qualityUpdateClassification|microsoft.graph.windowsUpdates.qualityUpdateClassification|A classificação na atualização de qualidade. Oferece suporte a um subconjunto dos valores **para qualityUpdateClassification**. Os valores possíveis são: `all`, `security`, `nonSecurity`. Somente leitura.|
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

