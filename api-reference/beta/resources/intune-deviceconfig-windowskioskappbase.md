---
title: tipo de recurso windowsKioskAppBase
description: A classe base de um tipo de aplicativo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c599a7d2c39ed573302507b812225a8d1783968c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466842"
---
# <a name="windowskioskappbase-resource-type"></a>tipo de recurso windowsKioskAppBase

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe base de um tipo de aplicativo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Propriedadesstartlayouttilesize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho do bloco do aplicativo para o layout inicial. Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|nome|String|Representa o nome amigável de um aplicativo|
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



