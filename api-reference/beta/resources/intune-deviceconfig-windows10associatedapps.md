---
title: tipo de recurso de windows10AssociatedApps
description: Definição de aplicativo do Windows 10 associados.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 097edb32ca01d673bb4d42802e8588edd20cf2d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869619"
---
# <a name="windows10associatedapps-resource-type"></a>tipo de recurso de windows10AssociatedApps

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Definição de aplicativo do Windows 10 associados.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tipo de aplicativo|[windows10AppType](../resources/intune-deviceconfig-windows10apptype.md)|Tipo de aplicativo. Os valores possíveis são: `desktop` e `universal`.|
|identificador|Cadeia de caracteres|Identificador.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





