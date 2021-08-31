---
title: Tipo de recurso windowsKioskProfile
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7703d10ae28e0700905fb1360be58404a656c3ef
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58799174"
---
# <a name="windowskioskprofile-resource-type"></a>Tipo de recurso windowsKioskProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|profileId|String|Chave da entidade.|
|profileName|Cadeia de caracteres|Esse é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu inicial e os usuários aos quais essa configuração de quiosque é atribuída.|
|appConfiguration|[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|A configuração do aplicativo que será usada para essa configuração de quiosque.|
|userAccountsConfiguration|[Coleção windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)|As contas de usuário que serão bloqueadas para essa configuração de quiosque. Essa coleção pode conter no máximo 100 elementos.|

## <a name="relationships"></a>Relações
Nenhum

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



