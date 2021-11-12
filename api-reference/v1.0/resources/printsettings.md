---
title: Tipo de recurso printSettings
description: Representa as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 11cba611772065f8c2014143f0c83b45eb6bd766
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944260"
---
# <a name="printsettings-resource-type"></a>Tipo de recurso printSettings

Namespace: microsoft.graph

Representa as configurações de todo o locatário para o serviço de Impressão Universal.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|documentConversionEnabled|Boolean|Especifica se a conversão de documento está habilitada para o locatário. Se a conversão de documentos estiver habilitada, o serviço de Impressão Universal converterá automaticamente documentos em um formato compatível com a impressora (xps para pdf) quando necessário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printSettings",
  "documentConversionEnabled": "Boolean"
}
```

