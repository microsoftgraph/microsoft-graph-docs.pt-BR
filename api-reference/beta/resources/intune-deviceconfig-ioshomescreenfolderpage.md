---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma página para uma pasta que contém aplicativos e clipes da Web na Tela Inicial.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8c2ab79ac9fd460638d4530240362ffe9536a542
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111184"
---
# <a name="ioshomescreenfolderpage-resource-type"></a>Tipo de recurso iosHomeScreenFolderPage

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma página para uma pasta que contém aplicativos e clipes da Web na Tela Inicial.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome da página da pasta|
|aplicativos|Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)|Uma lista de aplicativos e clipes da Web a ser exibida em uma página dentro de uma pasta. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
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
```



