---
title: tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80b0afb706a71ef8e0e3d4877fa7d0df822fe1d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788118"
---
# <a name="operatingsystemversionrange-resource-type"></a>tipo de recurso operatingSystemVersionRange

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Intervalo de versão do sistema operacional.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|A descrição desse intervalo (por exemplo, Builds 1702 válidos)|
|lowestVersion|Cadeia de caracteres|A versão mais antiga inclusive que este intervalo contém.|
|highestVersion|Cadeia de caracteres|A versão mais recente inclusive que este intervalo contém.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





