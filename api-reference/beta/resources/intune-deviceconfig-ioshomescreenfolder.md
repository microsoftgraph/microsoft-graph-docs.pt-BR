---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cde0e7ff573e82398123eca17dfa03af29c58ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946466"
---
# <a name="ioshomescreenfolder-resource-type"></a>Tipo de recurso iosHomeScreenFolder

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma pasta que contém as páginas de aplicativos na tela inicial


Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)|
|páginas|Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)|Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo. Este conjunto pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```




