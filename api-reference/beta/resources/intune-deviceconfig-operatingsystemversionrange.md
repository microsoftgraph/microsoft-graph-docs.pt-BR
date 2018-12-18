---
title: tipo de recurso de operatingSystemVersionRange
description: Intervalo de versão do sistema operacional.
author: tfitzmac
ms.openlocfilehash: b853e71b2d8f66d24122afb51cea97fc6a8f8d7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331161"
---
# <a name="operatingsystemversionrange-resource-type"></a>tipo de recurso de operatingSystemVersionRange

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Intervalo de versão do sistema operacional.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|A descrição deste intervalo (por exemplo, válido 1702 compilações)|
|lowestVersion|String|A menor inclusive versão que contém esse intervalo.|
|highestVersion|String|A versão inclusive maior que contém esse intervalo.|

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





