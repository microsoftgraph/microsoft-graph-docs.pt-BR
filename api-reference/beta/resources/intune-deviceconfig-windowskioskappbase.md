---
title: tipo de recurso de windowsKioskAppBase
description: A classe base para um tipo de aplicativos
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b13807fdb0319b3c9a15248fa2d50ffc46ac164
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977021"
---
# <a name="windowskioskappbase-resource-type"></a>tipo de recurso de windowsKioskAppBase

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A classe base para um tipo de aplicativos
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho de blocos de aplicativo para o layout de iniciar. Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|Cadeia de caracteres|Representa o nome amigável de um aplicativo|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String"
}
```





