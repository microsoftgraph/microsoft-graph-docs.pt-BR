---
title: Tipo de recurso androidDeviceOwnerKioskModeApp
description: Um aplicativo na Tela Inicial Gerenciada do Proprietário do Dispositivo Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e4012bff268811e264561076348d21a15cc98a0
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820503"
---
# <a name="androiddeviceownerkioskmodeapp-resource-type"></a>Tipo de recurso androidDeviceOwnerKioskModeApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um aplicativo na Tela Inicial Gerenciada do Proprietário do Dispositivo Android


Herda de [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|pacote|Cadeia de caracteres|Nome do pacote do aplicativo|
|className|Cadeia de caracteres|Nome da classe do aplicativo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeApp",
  "package": "String",
  "className": "String"
}
```



