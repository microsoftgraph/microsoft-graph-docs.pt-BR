---
title: Tipo de recurso ocrSettings
description: Representa as configurações de OCR para um caso de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e3951812e8196a4bd5839f5580cf79bac8bc671e
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838224"
---
# <a name="ocrsettings-resource-type"></a>Tipo de recurso ocrSettings

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de OCR (Reconhecimento Óptico de Caracteres) para um caso de Descoberta Eletrônica.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Indica se o OCR está habilitado ou não para o caso.|
|maxImageSize|Int32|Tamanho máximo da imagem que será processado em KB).|
|timeout|Duração|A duração do tempo limite para o mecanismo de OCR. Um tempo limite maior pode aumentar o sucesso do OCR, mas pode aumentar o tempo total de processamento.|

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

