---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém páginas de aplicativos e clipes da Web na Tela Inicial.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74c0f572b16dd10777cf2b429440f50237d4092e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786989"
---
# <a name="ioshomescreenfolder-resource-type"></a>Tipo de recurso iosHomeScreenFolder

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma pasta que contém páginas de aplicativos e clipes da Web na Tela Inicial.


Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)|
|páginas|Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)|Páginas de Ícones de Layout da Tela Inicial que devem ser aplicativos ou clipes da Web. Esta coleção pode conter um máximo de 500 elementos.|

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
          "bundleID": "String",
          "isWebClip": true
        }
      ]
    }
  ]
}
```



