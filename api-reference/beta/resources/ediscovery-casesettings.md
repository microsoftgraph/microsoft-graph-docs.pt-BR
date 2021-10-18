---
title: Tipo de recurso caseSettings
description: Contém ettings para um caso de Descoberta E.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 97b79952653c33d614276ca57c4b726a97cd9be4
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446452"
---
# <a name="casesettings-resource-type"></a>Tipo de recurso caseSettings

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém configurações para um caso de Descoberta E. Para obter detalhes, consulte [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter caseSettings](../api/ediscovery-casesettings-get.md)|[microsoft.graph.ediscovery.caseSettings](../resources/ediscovery-casesettings.md)|Leia as propriedades e as relações de um [objeto microsoft.graph.ediscovery.caseSettings.](../resources/ediscovery-casesettings.md)|
|[Atualizar caseSettings](../api/ediscovery-casesettings-update.md)|[microsoft.graph.ediscovery.caseSettings](../resources/ediscovery-casesettings.md)|Atualize as propriedades de [um objeto microsoft.graph.ediscovery.caseSettings.](../resources/ediscovery-casesettings.md)|
|[resetToDefault](../api/ediscovery-casesettings-resettodefault.md)|Nenhum|Redefinir todas as configurações para os valores padrão.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Id|Cadeia de caracteres|A ID do caso de Descoberta e. Herdado da [entidade](../resources/entity.md).|
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
  "@odata.type": "microsoft.graph.ediscovery.caseSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseSettings",
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
