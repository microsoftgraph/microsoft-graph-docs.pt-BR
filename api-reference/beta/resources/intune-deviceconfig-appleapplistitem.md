---
title: tipo de recurso appleAppListItem
description: Representa um aplicativo na lista de aplicativos Apple gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4804f3834a63a3c446c09d383c2244def97398
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470122"
---
# <a name="appleapplistitem-resource-type"></a>tipo de recurso appleAppListItem

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um aplicativo na lista de aplicativos Apple gerenciados


Herda de [appListItem](../resources/intune-deviceconfig-applistitem.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|O nome do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|publicador|String|O fornecedor do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|appStoreUrl|String|A URL da loja do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)|
|appId|String|O identificador do pacote do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



