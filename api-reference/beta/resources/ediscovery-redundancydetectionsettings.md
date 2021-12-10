---
title: Tipo de recurso redundancyDetectionSettings
description: Configurações de redundância para um caso de Descoberta E.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: ddd3d06e7d174509cae55fab0542a286fd4c1c70
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403167"
---
# <a name="redundancydetectionsettings-resource-type"></a>Tipo de recurso redundancyDetectionSettings

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Redundância (threading de email e detecção quase duplicada) para um caso de Descoberta Automática.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Indica se o threading de email e a detecção quase duplicada estão habilitados.|
|maxWords|Int32|Especifica o número máximo de palavras usadas para threading de email e detecção quase duplicada. Para saber mais, confira [Número mínimo/máximo de palavras](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|
|minWords|Int32|Especifica o número mínimo de palavras usadas para threading de email e detecção quase duplicada. Para saber mais, confira [Número mínimo/máximo de palavras](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|
|similarityThreshold|Int32|Especifica o nível de semelhança para que os documentos sejam colocados no mesmo conjunto quase duplicado. Para saber mais, confira [Limite de semelhança de documento e email.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```
