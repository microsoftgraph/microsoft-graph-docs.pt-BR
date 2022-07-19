---
title: Tipo de recurso redundancyDetectionSettings
description: Representa as configurações de redundância para um caso de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 3717992dc8cc9d1be843430c0a517f081e9bf220
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837524"
---
# <a name="redundancydetectionsettings-resource-type"></a>Tipo de recurso redundancyDetectionSettings

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de redundância (threading de email e detecção de duplicatas próximas) para um caso de Descoberta Eletrônica.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Indica se o threading de email e a detecção de duplicatas próximas estão habilitados.|
|maxWords|Int32|Especifica o número máximo de palavras usadas para threading de email e detecção de duplicatas próximas. Para saber mais, confira [o número mínimo/máximo de palavras](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|
|minWords|Int32|Especifica o número mínimo de palavras usadas para threading de email e detecção de duplicatas próximas. Para saber mais, confira [o número mínimo/máximo de palavras](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|
|similarityThreshold|Int32|Especifica o nível de similaridade para que os documentos sejam colocados no mesmo conjunto quase duplicado. Para saber mais, confira [o limite de similaridade de documentos e emails](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.redundancyDetectionSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```

