---
title: Tipo de recurso windowsKioskUWPApp
description: A classe base para um tipo de aplicativo
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ef0294701a660219a1c74119cc2af2912a315df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105969"
---
# <a name="windowskioskuwpapp-resource-type"></a>Tipo de recurso windowsKioskUWPApp

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
|autoLaunch|Boleano|Permitir que o aplicativo seja lançado automaticamente no modo de quiosque de vários aplicativos Herdado do [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appUserModelId|Cadeia de Caracteres|Esta é a única ID do Modelo de Usuário de Aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo Quiosque|
|appId|Cadeia de caracteres|Isso faz referência a um Aplicativo do Intune que será destinado às mesmas atribuições que a configuração do Quiosque|
|containedAppId|Cadeia de Caracteres|Isso faz referência a um aplicativo contido de um aplicativo do Intune|

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



