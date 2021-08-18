---
title: Tipo de recurso windowsKioskDesktopApp
description: A classe base para um tipo de aplicativo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44c83d125eaf7d29afe81948c187b142b8b23babd298bf11bb4f98a5952bb0d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133317"
---
# <a name="windowskioskdesktopapp-resource-type"></a>Tipo de recurso windowsKioskDesktopApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe base para um tipo de aplicativo


Herda do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho do azulejo do aplicativo para o layout inicial Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|nome|Cadeia de caracteres|Representa o nome amigável de um aplicativo Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|O tipo de aplicativo Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.|
|autoLaunch|Boolean|Permitir que o aplicativo seja lançado automaticamente no modo de quiosque de vários aplicativos Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|caminho|String|Definir o caminho de um aplicativo de área de trabalho|
|desktopApplicationId|Cadeia de caracteres|Definir o DesktopApplicationID do aplicativo|
|desktopApplicationLinkPath|Cadeia de caracteres|Definir o DesktopApplicationLinkPath do aplicativo|

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
  "appType": "String",
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




