---
title: tipo de recurso androidDeviceOwnerKioskModeAppPositionItem
description: Um item na lista de posições do aplicativo que define a ordem dos itens na Tela Inicial Gerenciada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06853e56c8c5620b4290cb385ada5ec938d79a71
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58813590"
---
# <a name="androiddeviceownerkioskmodeapppositionitem-resource-type"></a>tipo de recurso androidDeviceOwnerKioskModeAppPositionItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um item na lista de posições do aplicativo que define a ordem dos itens na Tela Inicial Gerenciada

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|position|Int32|Posição do item na grade. Valores válidos de 0 a 9999999|
|item|[androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)|Item a ser organizado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
  "position": 1024,
  "item": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
    "label": "String",
    "link": "String"
  }
}
```



