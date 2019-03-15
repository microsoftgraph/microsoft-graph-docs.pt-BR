---
title: tipo de recurso windowsKioskProfile
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f00d8cdb8030a29baccc4a8f29e6c6e562c900
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571946"
---
# <a name="windowskioskprofile-resource-type"></a>tipo de recurso windowsKioskProfile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ProfileId|String|Chave da entidade.|
|ProfileName|String|Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu iniciar e os usuários aos quais esta configuração de quiosque é atribuída.|
|appConfiguration|[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|A configuração do aplicativo que será usada para esta configuração de quiosque.|
|userAccountsConfiguration|coleção [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)|As contas de usuário que serão bloqueadas para esta configuração de quiosque. Essa coleção pode conter um máximo de 100 elementos.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
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
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```




