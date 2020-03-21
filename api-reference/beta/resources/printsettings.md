---
title: tipo de recurso printSettings
description: Representa configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 08d8409113c9c2f480200999c47ca18c300f245f
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895496"
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
