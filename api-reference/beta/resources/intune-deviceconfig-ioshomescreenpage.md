---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c726d751d81277a4f1b79a33606e1a2ec3eaede
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521604"
---
# <a name="ioshomescreenpage-resource-type"></a>Tipo de recurso iosHomeScreenPage

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma página que contém aplicativos e pastas na tela inicial

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome da página|
|ícones|Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)|Uma lista dos aplicativos e pastas exibidos em uma página. Este conjunto pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
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
  ]
}
```





