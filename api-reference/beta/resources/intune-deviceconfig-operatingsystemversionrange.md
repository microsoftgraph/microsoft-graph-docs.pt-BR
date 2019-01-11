---
title: tipo de recurso de operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56df6b53dc29247d3f718ad185152069a071a0f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875800"
---
# <a name="operatingsystemversionrange-resource-type"></a>tipo de recurso de operatingSystemVersionRange

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Intervalo de versão do sistema operacional.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|A descrição deste intervalo (por exemplo, válido 1702 compilações)|
|lowestVersion|Cadeia de caracteres|A menor inclusive versão que contém esse intervalo.|
|highestVersion|Cadeia de caracteres|A versão inclusive maior que contém esse intervalo.|

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





