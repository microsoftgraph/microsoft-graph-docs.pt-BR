---
title: tipo de recurso de windowsKioskAppBase
description: A classe base para um tipo de aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca86969eb32a1a1d129fb5ba4cd48bbb04ffd78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407141"
---
# <a name="windowskioskappbase-resource-type"></a>tipo de recurso de windowsKioskAppBase

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A classe base para um tipo de aplicativos

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|O tamanho de blocos de aplicativo para o layout de iniciar. Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Representa o nome amigável de um aplicativo|
|tipo de aplicativo|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|O tipo de aplicativo. Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.|

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
  "appType": "String"
}
```




