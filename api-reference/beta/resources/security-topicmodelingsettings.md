---
title: Tipo de recurso topicModelingSettings
description: Configurações de modelagem de tópico para um caso de Descoberta Eletrônica
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 865368b2d6d0723a47cc352e64f5400f254b3183
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945022"
---
# <a name="topicmodelingsettings-resource-type"></a>Tipo de recurso topicModelingSettings

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações de modelagem de tópico (Temas) para um caso de Descoberta Eletrônica. Para saber mais, confira [Definir configurações de pesquisa e análise na Descoberta Eletrônica Avançada](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|dynamicallyAdjustTopicCount|Booleano|Para saber mais, confira [Ajustar o número máximo de temas dinamicamente](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|
|ignoreNumbers|Booleano|Para saber mais, confira [Incluir números em temas](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|
|isEnabled|Booliano|Indica se os temas estão habilitados para o caso.|
|topicCount|Int32|Para saber mais, confira [o número máximo de temas](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.topicModelingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.topicModelingSettings",
  "isEnabled": "Boolean",
  "ignoreNumbers": "Boolean",
  "topicCount": "Integer",
  "dynamicallyAdjustTopicCount": "Boolean"
}
```

