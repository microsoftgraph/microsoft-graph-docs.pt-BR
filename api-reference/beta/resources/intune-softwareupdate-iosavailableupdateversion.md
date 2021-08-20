---
title: Tipo de recurso iosAvailableUpdateVersion
description: Detalhes da versão de atualização disponível do iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3174d0405785d31547f5b85bbd21d48598b9837783b97d0dd782b639ff43e7c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193507"
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
|supportedDevices|String collection|Lista de dispositivos com suporte para a atualização.|

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




