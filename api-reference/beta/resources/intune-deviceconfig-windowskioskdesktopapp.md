---
title: tipo de recurso de windowsKioskDesktopApp
description: A classe base para um tipo de aplicativos
author: tfitzmac
ms.openlocfilehash: a5ef4000b66f15f5951b49a152d25df30167004d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344517"
---
# <a name="windowskioskdesktopapp-resource-type"></a>tipo de recurso de windowsKioskDesktopApp

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A classe base para um tipo de aplicativos

Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho de blocos de aplicativo para o layout de iniciar Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Representa o nome amigável de um aplicativo Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|caminho|String|Definir o caminho de um aplicativo de área de trabalho|
|desktopApplicationId|String|Definir o DesktopApplicationID do aplicativo|
|desktopApplicationLinkPath|String|Definir o DesktopApplicationLinkPath do aplicativo|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





