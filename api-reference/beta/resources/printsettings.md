---
title: tipo de recurso printSettings
description: Representa configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c9af888d85256b88d4212cc84ba74d8dcdd5b590
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973817"
---
# <a name="printsettings-resource-type"></a>tipo de recurso printSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações de todo o locatário para o serviço de impressão universal.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|documentConversionEnabled|Boolean|Especifica se a conversão de documentos está habilitada para o locatário. Se a conversão de documentos estiver habilitada, o serviço de impressão universal converterá automaticamente os documentos em um formato compatível com a impressora (XPS para PDF), quando necessário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de printSettings.
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


