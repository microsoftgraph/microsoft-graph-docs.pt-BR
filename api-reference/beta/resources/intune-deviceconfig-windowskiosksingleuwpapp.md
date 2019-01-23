---
title: tipo de recurso de windowsKioskSingleUWPApp
description: A classe usada para identificar as informações de app UWP para a configuração de quiosque
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e62dc6393cc2dc6a9133732a42527abdfadbd91e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409374"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a>tipo de recurso de windowsKioskSingleUWPApp

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A classe usada para identificar as informações de app UWP para a configuração de quiosque


Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|uwpApp|[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)|Este é o único aplicativo usuário modelo ID (AUMID) que estarão disponíveis para uso no modo de quiosque de início|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




