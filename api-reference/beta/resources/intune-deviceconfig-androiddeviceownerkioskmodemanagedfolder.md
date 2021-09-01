---
title: Tipo de recurso androidDeviceOwnerKioskModeManagedFolder
description: Uma pasta que contém páginas de aplicativos e weblinks na Tela Inicial Gerenciada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6144091708f3abfea6aa0f8e0b4ac7284cf58580
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787024"
---
# <a name="androiddeviceownerkioskmodemanagedfolder-resource-type"></a>Tipo de recurso androidDeviceOwnerKioskModeManagedFolder

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma pasta que contém páginas de aplicativos e weblinks na Tela Inicial Gerenciada

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|folderName|Cadeia de caracteres|Nome para exibição da pasta|
|folderIdentifier|Cadeia de caracteres|Identificador exclusivo da pasta|
|itens|[coleção androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)|Itens a serem adicionados à pasta gerenciada. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
  "folderName": "String",
  "folderIdentifier": "String",
  "items": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
      "label": "String",
      "link": "String"
    }
  ]
}
```



