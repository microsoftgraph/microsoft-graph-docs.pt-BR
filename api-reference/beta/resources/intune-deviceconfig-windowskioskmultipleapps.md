---
title: tipo de recurso tipo complexowindowskioskmultipleapps
description: A classe usada para identificar a configuração do aplicativo multimodo para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 010f8196bd152b872b3910eec9759e31efa4a1e1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463454"
---
# <a name="windowskioskmultipleapps-resource-type"></a>tipo de recurso tipo complexowindowskioskmultipleapps

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe usada para identificar a configuração do aplicativo multimodo para a configuração do quiosque


Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|apps|coleção [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|Estes são os únicos aplicativos da Windows Store que estarão disponíveis para inicialização no menu iniciar. Essa coleção pode conter um máximo de 128 elementos.|
|a barra de tarefas|Booliano|Essa configuração permite que o administrador especifique se a barra de tarefas é mostrada ou não.|
|allowAccessToDownloadsFolder|Booliano|Essa configuração permite o acesso à pasta downloads no explorador de arquivos.|
|disallowDesktopApps|Booliano|Essa configuração indica que os aplicativos de área de trabalho são permitidos. O padrão é true.|
|startMenuLayoutXml|Binária|Permite que os administradores substituam o layout de início padrão e impede que o usuário o altere.O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout. XML precisa estar no formato binário.|

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
      "appType": "String",
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```



