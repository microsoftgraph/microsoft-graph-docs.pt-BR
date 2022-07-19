---
title: Tipo de recurso ediscoveryCaseSettings
description: Contém configurações para um caso de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 9ddca3073403ea284295d89bbf4dae3fe4e380c4
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839040"
---
# <a name="ediscoverycasesettings-resource-type"></a>Tipo de recurso ediscoveryCaseSettings

Namespace: microsoft.graph.security



Contém configurações para um caso de Descoberta Eletrônica. Para obter detalhes, [consulte Definir configurações de pesquisa e análise na Descoberta Eletrônica (Premium)](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter ediscoveryCaseSettings](../api/security-ediscoverycasesettings-get.md)|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|Leia as propriedades e as relações de [um objeto ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md) .|
|[Atualizar ediscoveryCaseSettings](../api/security-ediscoverycasesettings-update.md)|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|Atualize as propriedades de [um objeto ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md) .|
|[resetToDefault](../api/security-ediscoverycasesettings-resettodefault.md)|Nenhum|Redefina todas as configurações para os valores padrão.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID do caso de Descoberta Eletrônica. Herdado da [entidade](../resources/entity.md).|
|Ocr|[microsoft.graph.security.ocrSettings](../resources/security-ocrsettings.md)|As configurações de OCR (Reconhecimento Óptico de Caracteres) para o caso.|
|redundancyDetection|[microsoft.graph.security.redundancyDetectionSettings](../resources/security-redundancydetectionsettings.md)|As configurações de detecção de redundância (quase duplicados e threading de email) para o caso.|
|topicModeling|[microsoft.graph.security.topicModelingSettings](../resources/security-topicmodelingsettings.md)|As configurações de Modelagem de Tópico (Temas) para o caso.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCaseSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCaseSettings",
  "id": "String (identifier)",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.security.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.security.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.security.ocrSettings"
  }
}
```

