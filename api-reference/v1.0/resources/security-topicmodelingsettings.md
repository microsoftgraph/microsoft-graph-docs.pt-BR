---
title: Tipo de recurso topicModelingSettings
description: Representa as configurações de modelagem de tópico para um caso de Descoberta Eletrônica
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a021febfda5cd37845f8423de60e0a5a5782325e
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839046"
---
# <a name="topicmodelingsettings-resource-type"></a>Tipo de recurso topicModelingSettings

Namespace: microsoft.graph.security



Representa as configurações de modelagem de tópico (Temas) para um caso de Descoberta Eletrônica. Para saber mais, confira [Definir configurações de pesquisa e análise na Descoberta Eletrônica (Premium)](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|dynamicallyAdjustTopicCount|Booliano|Indica se o modelo de temas deve otimizar dinamicamente o número de tópicos gerados. Para saber mais, confira [Ajustar o número máximo de temas dinamicamente](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|
|ignoreNumbers|Booliano|Indica se o modelo de temas deve excluir números ao analisar textos de documento. Para saber mais, confira [Incluir números em temas](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|
|isEnabled|Booliano|Indica se o modelo de temas está habilitado para o caso.|
|topicCount|Int32|O número total de tópicos que o modelo de temas gerará para um conjunto de revisão. Para saber mais, confira [o número máximo de temas](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|

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

