---
title: tipo de recurso iosAvailableUpdateVersion
description: detalhes da versão da atualização disponível do iOS
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29cf7500bc7069af0b2a1184adb0fe28bb0ac891
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766361"
---
# <a name="iosavailableupdateversion-resource-type"></a>tipo de recurso iosAvailableUpdateVersion

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

detalhes da versão da atualização disponível do iOS

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|productVersion|String|A versão da atualização.|
|postingDateTime|DateTimeOffset|A data de lançamento da atualização.|
|expirationDateTime|DateTimeOffset|A data de expiração da atualização.|
|supportedDevices|Coleção de cadeias de caracteres|Lista de dispositivos com suporte para a atualização.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "productVersion": "String",
  "postingDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "supportedDevices": [
    "String"
  ]
}
```



