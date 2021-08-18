---
title: Tipo de recurso windowsKioskWin32App
description: Suporte a aplicativos do KioskModeApp v4 para Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb0d9a7a14456740872c9eac193522e8113dc5c91acea4c44e235a1c3e0449ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164262"
---
# <a name="windowskioskwin32app-resource-type"></a>Tipo de recurso windowsKioskWin32App

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Suporte a aplicativos do KioskModeApp v4 para Win32


Herda do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho do azulejo do aplicativo para o layout inicial Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|nome|Cadeia de caracteres|Representa o nome amigável de um aplicativo Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|O tipo de aplicativo Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean|Permitir que o aplicativo seja lançado automaticamente no modo de quiosque de vários aplicativos Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|classicAppPath|Cadeia de caracteres|Este é o classicapppath a ser usado pelo aplicativo v4 Win32 enquanto estiver no modo Quiosque|
|edgeNoFirstRun|Boolean|Sinalizador de primeira corrida de borda para o modo de quiosque de borda|
|edgeKioskIdleTimeoutMinutes|Int32|Tempo limite ocioso do quiosque de borda em minutos para o modo quiosque de Borda. Valores válidos de 0 a 1440|
|edgeKioskType|[windowsEdgeKioskType](../resources/intune-deviceconfig-windowsedgekiosktype.md)|Tipo de quiosque de borda para modo quiosque de borda. Os valores possíveis são: `publicBrowsing` e `fullScreen`.|
|edgeKiosk|Cadeia de caracteres|Quiosque de borda (url) para o modo de quiosque de borda|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskWin32App",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "classicAppPath": "String",
  "edgeNoFirstRun": true,
  "edgeKioskIdleTimeoutMinutes": 1024,
  "edgeKioskType": "String",
  "edgeKiosk": "String"
}
```




