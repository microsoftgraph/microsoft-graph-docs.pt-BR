---
title: Tipo de recurso ocrSettings
description: Configurações de OCR para um caso de Descoberta e
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 648e0ad63f558f211591d1c8aa976c2689dd271d
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080716"
---
# <a name="ocrsettings-resource-type"></a>Tipo de recurso ocrSettings

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações OCR (Reconhecimento Óptico de Caracteres) para o caso de Descoberta e.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Indica se o OCR está habilitado ou não para o caso.|
|maxImageSize|Int32|Tamanho máximo da imagem que será processado em KB).|
|timeout|Duration|A duração do tempo de duração do mecanismo OCR. Um tempo de tempo maior pode aumentar o sucesso do OCR, mas pode adicionar ao tempo total de processamento.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```
