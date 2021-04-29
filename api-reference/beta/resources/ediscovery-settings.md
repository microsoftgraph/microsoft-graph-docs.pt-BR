---
title: tipo de recurso de configurações (Descoberta eDiscovery)
description: Configurações para um caso de Descoberta E
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 9f0248fa0c6080a143272d997b9d6125e0ccb5a2
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080712"
---
# <a name="settings-resource-type-ediscovery"></a>tipo de recurso de configurações (Descoberta eDiscovery)

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações para um caso de Descoberta E. Para obter detalhes, consulte [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter configurações](../api/ediscovery-settings-get.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|Leia as propriedades e as relações de um [objeto microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md)|
|[Atualizar configurações](../api/ediscovery-settings-update.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|Atualize as propriedades de [um objeto microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md)|
|[resetToDefault](../api/ediscovery-settings-resettodefault.md)|Nenhum|Redefinir todas as configurações para os valores padrão.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Id|Cadeia de Caracteres|A ID do caso de Descoberta e. Herdado da [entidade](../resources/entity.md).|
|ocr|[microsoft.graph.ediscovery.ocrSettings](../resources/ediscovery-ocrsettings.md)|As configurações OCR (Reconhecimento Óptico de Caracteres) para a ocorrência.|
|redundancyDetection|[microsoft.graph.ediscovery.redundancyDetectionSettings](../resources/ediscovery-redundancydetectionsettings.md)|As configurações de detecção de redundância (quase duplicata e threading de email) para o caso.|
|topicModeling|[microsoft.graph.ediscovery.topicModelingSettings](../resources/ediscovery-topicmodelingsettings.md)|As configurações de Modelagem de Tópicos (Temas) para o caso.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.settings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.settings",
  "id": "String (identifier)",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
  }
}
```
