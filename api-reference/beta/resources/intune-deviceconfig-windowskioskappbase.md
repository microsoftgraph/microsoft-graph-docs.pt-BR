---
title: tipo de recurso windowsKioskAppBase
description: A classe base de um tipo de aplicativo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b86921fcdaa11b37b985184dfbc645c2a193bfdb
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572303"
---
# <a name="windowskioskappbase-resource-type"></a>tipo de recurso windowsKioskAppBase

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe base de um tipo de aplicativo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Propriedadesstartlayouttilesize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho do bloco do aplicativo para o layout inicial. Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|nome|String|Representa o nome amigável de um aplicativo|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|O tipo de aplicativo. Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.|
|autoLançamento|Boolean|Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos|

## <a name="relationships"></a>Relações
Nenhuma

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




