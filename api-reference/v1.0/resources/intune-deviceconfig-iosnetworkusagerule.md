---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
localization_priority: Normal
ms.openlocfilehash: 85b01c4cca324c0c344cc837da117efa05ae0ae4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845764"
---
# <a name="iosnetworkusagerule-resource-type"></a>Tipo de recurso iosNetworkUsageRule

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|managedApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará. Essa coleção pode conter um máximo de 500 elementos.|
|cellularDataBlockWhenRoaming|Booliano|Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.|
|cellularDataBlocked|Booliano|Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



