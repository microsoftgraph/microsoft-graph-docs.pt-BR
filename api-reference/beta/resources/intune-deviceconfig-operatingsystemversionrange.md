---
title: Tipo de recurso operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7a57dc5a1c7702cd4e0d2623ac2b0d54571a5d3a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58798108"
---
# <a name="operatingsystemversionrange-resource-type"></a>Tipo de recurso operatingSystemVersionRange

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Intervalo de versão do sistema operacional.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|A descrição desse intervalo (por exemplo, builds válidos 1702)|
|lowestVersion|Cadeia de caracteres|A versão inclusiva mais baixa que esse intervalo contém.|
|highestVersion|Cadeia de caracteres|A versão inclusiva mais alta que esse intervalo contém.|

## <a name="relationships"></a>Relações
Nenhum

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



