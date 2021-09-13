---
title: Tipo de recurso windowsKioskSingleUWPApp
description: A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c02df0ba696f00b99a449e90d04e0923a300fb30
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095455"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a>Tipo de recurso windowsKioskSingleUWPApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque


Herda do [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|uwpApp|[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)|Esta é a única ID do Modelo de Usuário de Aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo Quiosque|

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
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```



