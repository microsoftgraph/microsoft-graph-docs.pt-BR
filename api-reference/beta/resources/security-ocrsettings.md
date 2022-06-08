---
title: Tipo de recurso ocrSettings
description: Configurações de OCR para um caso de Descoberta Eletrônica
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d3a72dbcbdf75abe0e2da50aa8626a828a4d2588
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945028"
---
# <a name="ocrsettings-resource-type"></a>Tipo de recurso ocrSettings

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações de OCR (Reconhecimento Óptico de Caracteres) para o caso de Descoberta Eletrônica.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Indica se o OCR está habilitado ou não para o caso.|
|maxImageSize|Int32|Tamanho máximo da imagem que será processado em KB).|
|timeout|Duration|A duração do tempo limite para o mecanismo de OCR. Um tempo limite maior pode aumentar o sucesso do OCR, mas pode aumentar o tempo total de processamento.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.ocrSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```

