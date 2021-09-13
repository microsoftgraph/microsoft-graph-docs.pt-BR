---
title: Tipo de recurso iosAvailableUpdateVersion
description: Detalhes da versão de atualização disponível do iOS
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5ee887ea5e8e53b65ac0f83da331f6f8cb774f71
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029938"
---
# <a name="iosavailableupdateversion-resource-type"></a>Tipo de recurso iosAvailableUpdateVersion

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Detalhes da versão de atualização disponível do iOS

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|productVersion|String|A versão da atualização.|
|postingDateTime|DateTimeOffset|A data de postagem da atualização.|
|expirationDateTime|DateTimeOffset|A data de expiração da atualização.|
|supportedDevices|Conjunto de cadeias de caracteres|Lista de dispositivos com suporte para a atualização.|

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



