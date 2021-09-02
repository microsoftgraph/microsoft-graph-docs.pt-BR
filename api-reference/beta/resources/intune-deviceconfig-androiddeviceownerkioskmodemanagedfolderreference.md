---
title: Tipo de recurso androidDeviceOwnerKioskModeManagedFolderReference
description: Uma referência à pasta que contém aplicativos e weblinks na Tela Inicial Gerenciada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bcdb62a5c8ebf740b9c9f0060289af0ebded8ff3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819217"
---
# <a name="androiddeviceownerkioskmodemanagedfolderreference-resource-type"></a>Tipo de recurso androidDeviceOwnerKioskModeManagedFolderReference

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma referência à pasta que contém aplicativos e weblinks na Tela Inicial Gerenciada


Herda de [androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|folderName|Cadeia de caracteres|Nome da pasta|
|folderIdentifier|Cadeia de caracteres|Identificador exclusivo da pasta|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference",
  "folderName": "String",
  "folderIdentifier": "String"
}
```



