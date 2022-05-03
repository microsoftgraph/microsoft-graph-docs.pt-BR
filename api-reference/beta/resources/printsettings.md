---
title: Tipo de recurso printSettings
description: Representa as configurações de todo o locatário para o serviço de Impressão Universal.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0339843083695904080104882ba9385a840b4c9e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176652"
---
# <a name="printsettings-resource-type"></a>Tipo de recurso printSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de todo o locatário para o serviço de Impressão Universal.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|documentConversionEnabled|Booliano|Especifica se a conversão de documento está habilitada para o locatário. Se a conversão de documentos estiver habilitada, o Serviço de Impressão Universal converterá automaticamente documentos em um formato compatível com a impressora (xps para pdf) quando necessário.|

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de printSettings.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printSettings"
}-->

```json
{
  "documentConversionEnabled": true
}
```


