---
title: tipo de recurso windowsKioskUWPApp
description: A classe base de um tipo de aplicativo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9340006ee74e640e21dc6bef99cc1f0e297999b9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943771"
---
# <a name="windowskioskuwpapp-resource-type"></a>tipo de recurso windowsKioskUWPApp

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe base de um tipo de aplicativo


Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Propriedadesstartlayouttilesize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho do bloco do aplicativo para o layout inicial herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|nome|String|Representa o nome amigável de um aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|O tipo de aplicativo herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.|
|autolançamento|Booliano|Permitir que o aplicativo seja iniciado automaticamente no modo de quiosque de vários aplicativos herdado de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appUserModelId|Cadeia de caracteres|Esta é a única ID de modelo de usuário do aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo quiosque|
|appId|Cadeia de caracteres|Isso faz referência a um aplicativo do Intune que será direcionado para as mesmas atribuições como configuração de quiosque|
|containedAppId|Cadeia de caracteres|Isso faz referência a um aplicativo contido de um aplicativo do Intune|

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
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




