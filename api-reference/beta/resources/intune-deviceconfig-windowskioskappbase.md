---
title: tipo de recurso windowsKioskAppBase
description: A classe base de um tipo de aplicativo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dc6c54c9b788ae3456017fc0be63c636d980af8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993961"
---
# <a name="windowskioskappbase-resource-type"></a>tipo de recurso windowsKioskAppBase

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe base de um tipo de aplicativo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Propriedadesstartlayouttilesize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho do bloco do aplicativo para o layout inicial. Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Representa o nome amigável de um aplicativo|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|O tipo de aplicativo. Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.|
|autolançamento|Booliano|Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos|

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
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```





