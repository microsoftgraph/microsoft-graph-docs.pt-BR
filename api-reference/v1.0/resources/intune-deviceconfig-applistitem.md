---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0b9d7df95ce8ddb71439763eb02b205772e06300
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820318"
---
# <a name="applistitem-resource-type"></a>Tipo de recurso appListItem

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa um aplicativo na lista de aplicativos gerenciados
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|Cadeia de caracteres|O nome do aplicativo|
|distribuidor|Cadeia de caracteres|O distribuidor do aplicativo|
|appStoreUrl|Cadeia de caracteres|A URL da loja do aplicativo|
|appId|Cadeia de caracteres|O aplicativo ou identificador do pacote do aplicativo|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



