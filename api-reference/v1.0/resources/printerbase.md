---
title: Tipo de recurso printerBase
description: Representa o tipo base para o compartilhamento de impressora e impressora
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9e770cd0dfdd29da549114ca5a688718e679855c
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944981"
---
# <a name="printerbase-resource-type"></a>Tipo de recurso printerBase

Namespace: microsoft.graph

Representa um tipo de base para [tipos de](printer.md) entidade printer e [printerShare.](printerShare.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora/printerShare.|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão de printer/printerShare.|
|displayName|Cadeia de caracteres|O nome da impressora/printerShare.|
|id|Cadeia de caracteres|O identificador.|
|isAcceptingJobs|Boolean|Se a impressora/printerShare está aceitando novos trabalhos de impressão no momento.|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora/printerShare.|
|fabricante|String|O fabricante da impressora/printerShare.|
|modelo|String|O nome do modelo da impressora/printerShare.|
|status|[printerStatus](printerstatus.md)|O status de processamento da impressora/printerShare, incluindo quaisquer erros.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|jobs|[Coleção printJob](printjob.md)|A lista de trabalhos que estão na fila para impressão pela impressora/printerShare.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerBase",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  }
}
```

