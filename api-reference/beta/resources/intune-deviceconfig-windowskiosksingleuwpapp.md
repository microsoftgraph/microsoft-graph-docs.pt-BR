---
title: tipo de recurso windowsKioskSingleUWPApp
description: A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0a3b56c7bc9856b98708b63c247479e6ccf9c9b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571155"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a>tipo de recurso windowsKioskSingleUWPApp

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque


Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|uwpApp|[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)|Esta é a única ID de modelo de usuário do aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo quiosque|

## <a name="relationships"></a>Relações
Nenhuma

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
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




