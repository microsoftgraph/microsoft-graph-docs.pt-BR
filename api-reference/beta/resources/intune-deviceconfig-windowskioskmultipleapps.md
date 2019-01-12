---
title: tipo de recurso de windowsKioskMultipleApps
description: A classe usada para identificar a configuração de vários modos app para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3770f8c63be230dff97e43d3706ed35d79826751
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977126"
---
# <a name="windowskioskmultipleapps-resource-type"></a>tipo de recurso de windowsKioskMultipleApps

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A classe usada para identificar a configuração de vários modos app para a configuração de quiosque

Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Aplicativos|coleção [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|Estes são os únicos repositório aplicativos do Windows que estarão disponíveis para início no menu Iniciar.|
|showTaskBar|Booliano|Essa configuração permite que o administrador especificar se a barra de tarefas é mostrada ou não.|
|disallowDesktopApps|Booliano|Essa configuração indica que os aplicativos da área de trabalho são permitidos. Definido como true.|
|startMenuLayoutXml|Binária|Permite que os administradores substituir o layout de início padrão e impede que o usuário alterá-la.O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout. XML deve estar em formato binário.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





