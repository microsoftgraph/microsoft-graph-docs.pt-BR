---
title: Tipo de recurso printerBase
description: Representa o tipo base para o compartilhamento de impressora e impressora
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 12b611e73fab82d0ac1eafbdc19b26069ccfd94fa3806e4286da0f0c6516202b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235370"
---
# <a name="printerbase-resource-type"></a>Tipo de recurso printerBase

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa um tipo de base para [tipos de](printer.md) entidade printer e [printerShare.](printerShare.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora/printerShare.|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão de printer/printerShare.|
|displayName|Cadeia de caracteres|O nome da impressora/printerShare.|
|id|String|O identificador.|
|isAcceptingJobs|Booliano|Se a impressora/printerShare está aceitando novos trabalhos de impressão no momento.|
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

