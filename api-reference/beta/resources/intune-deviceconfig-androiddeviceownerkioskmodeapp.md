---
title: Tipo de recurso androidDeviceOwnerKioskModeApp
description: Um aplicativo na Tela Inicial Gerenciada do Proprietário do Dispositivo Android
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da86af4248136fe35f0674834113c98ae580bf45
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106592"
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
|pacote|Cadeia de Caracteres|Nome do pacote do aplicativo|
|className|Cadeia de Caracteres|Nome da classe do aplicativo|

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



