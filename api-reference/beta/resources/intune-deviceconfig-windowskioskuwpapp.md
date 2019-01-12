---
title: tipo de recurso de windowsKioskUWPApp
description: A classe base para um tipo de aplicativos
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8719fdd248276a657b96235c592f1bb62607b856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934909"
---
# <a name="windowskioskuwpapp-resource-type"></a>tipo de recurso de windowsKioskUWPApp

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A classe base para um tipo de aplicativos

Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho de blocos de aplicativo para o layout de iniciar Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|Cadeia de caracteres|Representa o nome amigável de um aplicativo Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appUserModelId|Cadeia de caracteres|Este é o único aplicativo usuário modelo ID (AUMID) que estarão disponíveis para uso no modo de quiosque de início|
|appId|Cadeia de caracteres|Isso faz referência a um App Intune que será o destino para as atribuições mesmos como a configuração de quiosque|
|containedAppId|Cadeia de caracteres|Isso faz referência a um aplicativo contido de um App Intune|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





