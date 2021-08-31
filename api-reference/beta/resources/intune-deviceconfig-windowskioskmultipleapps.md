---
title: Tipo de recurso windowsKioskMultipleApps
description: A classe usada para identificar a configuração do aplicativo MultiMode para a configuração de quiosque
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 678943374b2db49513ca0739f75cead5565ce99c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800405"
---
# <a name="windowskioskmultipleapps-resource-type"></a>Tipo de recurso windowsKioskMultipleApps

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe usada para identificar a configuração do aplicativo MultiMode para a configuração de quiosque


Herda do [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|apps|[Coleção windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|Esses são os únicos Windows aplicativos da Loja que estarão disponíveis para iniciar a partir do menu Iniciar. Essa coleção pode conter no máximo 128 elementos.|
|showTaskBar|Boleano|Essa configuração permite que o administrador especifique se a Barra de Tarefas será exibida ou não.|
|allowAccessToDownloadsFolder|Boleano|Essa configuração permite o acesso à pasta Downloads no explorador de arquivos.|
|disallowDesktopApps|Boleano|Essa configuração indica que os aplicativos da área de trabalho são permitidos. Padrão para true.|
|startMenuLayoutXml|Binária|Permite que os administradores substituam o layout de início padrão e impedem que o usuário o mude. O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout. XML precisa estar no formato Binário.|

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



